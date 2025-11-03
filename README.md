# 📚 FAFSA Household Support Worksheet

**An Interactive Learning Tool for FAFSA Family Size Calculation**

[![Version](https://img.shields.io/badge/version-2.0-blue.svg)](https://github.com/ThiinkMG/fafsa-household-support-worksheet)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-production-brightgreen.svg)](https://github.com/ThiinkMG/fafsa-household-support-worksheet)

---

## 🎯 Overview

The **FAFSA Household Support Worksheet** is a comprehensive, interactive web application designed to help students accurately calculate their FAFSA family size and understand complex financial aid eligibility rules. This tool transforms a traditionally confusing process into an engaging learning experience.

### Try it out

[Try FAFSA Household Support Worksheet (Online Link)](https://thiinkmg.github.io/FAFSA-Household-Size-and-Support-Worksheet)

---

### Key Features

✅ **Interactive Learning System**
- Real-time tooltips explaining FAFSA terminology
- Knowledge check quizzes to reinforce understanding
- Educational error validation with helpful tips
- Resource hub with official FAFSA.gov links

✅ **Smart Calculations**
- Live running tally showing family size & college enrollment
- Automatic updates as you input data
- Validation to catch common mistakes
- Multi-year academic year selector (2024-2029)

✅ **Professional Tools**
- Auto-save to localStorage (never lose progress)
- PDF export (blank template + completed worksheet)
- Dark mode support
- Fully responsive mobile design

---

## 🚀 Quick Start

### For Students

1. **Open the worksheet**: Simply open `index.html` in any modern web browser
2. **Select your academic year**: Choose the FAFSA year you're applying for
3. **Fill out your information**: Follow the guided sections
4. **Learn as you go**: Hover over blue ℹ️ icons to learn FAFSA terms
5. **Export your results**: Download a PDF when complete

### For Developers

```bash
# Clone the repository
git clone https://github.com/ThiinkMG/fafsa-household-support-worksheet.git

# Navigate to the directory
cd fafsa-household-support-worksheet

# Open in browser
open index.html
```

**No build process required!** This is a standalone HTML file with embedded CSS and JavaScript.

---

## 📊 What's Included

### File Structure

```
fafsa-household-support-worksheet/
├── index.html                              # Main application (2,600+ lines)
├── README.md                               # This file
├── ENHANCEMENT-PLAN.md                     # Full feature roadmap
├── IMPLEMENTATION-SUMMARY.md               # Development changelog
├── QUICK-START-GUIDE.md                    # Implementation guide
├── MCF_FAFSA_Household_Worksheet_BLANK_TEMPLATE.pdf
├── create_template.py                      # PDF generation script
├── images/                                 # Screenshots & assets
└── archive/                                # Previous versions
```

---

## 🎓 Learning Features

### 1. Hover Tooltip System
**15+ Interactive Tooltips** explaining key FAFSA concepts:
- Family Size definition
- 51% support rule with examples
- Half-time enrollment requirements
- Academic year vs tax year differences
- Dependent vs Independent status

**Example:**
```html
<span class="tooltip-trigger">
  ℹ️
  <span class="tooltip-popup">
    <strong>The 51% Support Rule</strong>
    <span>To include someone in your household, you must provide
    MORE THAN HALF of their living expenses...</span>
  </span>
</span>
```

### 2. Running Tally Display
Real-time calculations visible at all times:
- **Family Size**: Auto-calculated as you add members
- **Number in College**: Live count of enrolled students
- **Status Indicator**: Shows completion progress

**Responsive Design:**
- Desktop: Sticky sidebar on right
- Mobile: Fixed bottom bar

### 3. Knowledge Check Quizzes
**2 Interactive Quizzes** strategically placed after key sections:

**Quiz 1**: After Family Size Section
- Tests understanding of the 51% support rule
- Includes real-world scenarios (e.g., grandmother on Social Security)

**Quiz 2**: After Number in College Section
- Clarifies who counts in college enrollment
- Prevents common mistake of including parents

### 4. Smart Error Validation
Educational error messages that teach, not just correct:

**Example Error:**
```
⚠️ Error Detected
You entered 3 people in college, but your family size is only 2.
This isn't possible!

💡 Tip: Count everyone in Part 1 first, then count how many of
THOSE people are in college in Part 2.
```

### 5. Resource Hub
Collapsible section with 5 official FAFSA.gov links:
- Family Size Definition (2025-2026)
- Number in College Guidance
- Dependency Status Rules
- Historical FAFSA terminology changes
- Official glossary

### 6. Academic Year Selector
**Dynamic year selection** with automatic updates:
- Choose from 2024-2029 academic years
- Automatically calculates correct tax year (prior-prior year formula)
- Updates all date references throughout worksheet
- Tax year = Academic Start Year - 2

**Example:**
- 2025-2026 Academic Year → Uses 2023 Tax Data (filed in 2024)
- 2026-2027 Academic Year → Uses 2024 Tax Data (filed in 2025)

---

## 🎨 Design System

### MCF Brand Colors
```css
--mcf-brand-blue:  #012699  /* Primary brand color */
--mcf-brand-green: #26e011  /* Success states */
--mcf-brand-amber: #fdc003  /* Warnings & tips */
--mcf-brand-black: #000516  /* Text & headings */
```

### Dark Mode Support
Automatic color scheme switching for comfortable viewing in any environment.

### Responsive Breakpoints
- **Desktop**: Full sidebar layout, hover tooltips
- **Mobile (≤768px)**: Stacked layout, tap tooltips, bottom tally bar

---

## 💾 Technical Features

### Auto-Save System
All data automatically saved to browser's `localStorage`:
- Student information
- Household members
- Academic year selection
- Resource hub collapse state
- Progress tracking

**Storage Key:** `mcf-fafsa-worksheet-state`

### PDF Export
Two export options:
1. **Blank Template**: Empty worksheet for printing
2. **Completed Worksheet**: Pre-filled with your data

**Includes:**
- Student information
- All household members
- Calculated family size & college count
- Professional formatting
- MCF branding

### Browser Compatibility
✅ Chrome 90+
✅ Firefox 88+
✅ Safari 14+
✅ Edge 90+

**Technologies Used:**
- Vanilla JavaScript (no dependencies)
- CSS3 with custom properties
- HTML5 semantic markup
- LocalStorage API
- Print media queries

---

## 📈 Statistics

| Metric | Value |
|--------|-------|
| **Total Lines of Code** | 2,600+ |
| **Interactive Tooltips** | 15+ |
| **Knowledge Checks** | 2 quizzes |
| **Validation Rules** | 4+ |
| **Academic Years** | 5 (2024-2029) |
| **Official Links** | 5 FAFSA.gov resources |
| **Load Time** | < 1 second |
| **File Size** | ~96 KB (single HTML file) |

---

## 🎯 Learning Outcomes

After completing this worksheet, students will understand:

✅ **FAFSA Dependency Status**
- Difference between dependent and independent students
- How status affects family size calculation

✅ **The 51% Support Rule**
- How to calculate if you provide majority support
- Examples of support categories (housing, food, medical, etc.)

✅ **Family Size Calculation**
- Who counts in your FAFSA household
- Who does NOT count (roommates, relatives with own income)

✅ **Number in College**
- Who can be included in college enrollment count
- Why parents don't count (common mistake)

✅ **Aid Year vs Tax Year**
- Understanding "prior-prior year" tax data
- Why 2025-2026 FAFSA uses 2023 taxes

---

## 🛠️ Development

### Enhancement History

**Phase 1 & 2 (Completed):**
- ✅ Hover tooltip system
- ✅ Running tally display
- ✅ Knowledge check questions
- ✅ Error validation with education
- ✅ Academic year selector
- ✅ Resource hub section

**Phase 3 (Future):**
- [ ] Dependency status quiz (11-question interactive)
- [ ] What-if scenario mode
- [ ] Enhanced PDF with calculation breakdown
- [ ] Analytics tracking (optional)

### Code Structure

**CSS (Lines 7-1100):**
- MCF brand variables
- Dark mode overrides
- Tooltip system
- Running tally box
- Knowledge checks
- Resource hub
- Responsive media queries

**HTML (Lines 1101-2000):**
- Hero section with dynamic dates
- Student information form
- Household member cards
- Section A & B (family size)
- Knowledge checks
- Final reminders
- Resource hub

**JavaScript (Lines 2001-2600):**
- State management
- Auto-save functionality
- PDF generation
- Running tally calculations
- Tooltip interactions
- Knowledge check logic
- Academic year updates
- Dark mode toggle

---

## 📝 Usage Examples

### Example 1: Dependent Student
```
Academic Year: 2025-2026
Status: Dependent
Family Size: 4
  - Student (you): 1
  - Parents: 2
  - Sibling (lives at home): 1
Number in College: 2
  - Student (you): 1
  - Sibling (enrolled half-time+): 1
```

### Example 2: Independent Student
```
Academic Year: 2026-2027
Status: Independent
Family Size: 3
  - Student (you): 1
  - Spouse: 1
  - Your child: 1
Number in College: 1
  - Student (you): 1
```

---

## 🚨 Common Mistakes Prevented

This tool helps students avoid these frequent errors:

❌ **Including people with their own income**
- Relatives who support themselves don't count

❌ **Counting parents in "Number in College"**
- Only students working toward first bachelor's degree count

❌ **More people in college than family size**
- Logical impossibility caught by validation

❌ **Wrong tax year**
- Automatic calculation based on academic year

❌ **Forgetting the 51% rule**
- Tooltips and quizzes reinforce this constantly

---

## 📞 Support Resources

### Official FAFSA Links (Built-in)
All links open in new tab for easy reference:
- [Family Size Definition](https://studentaid.gov/2526/help/family-size)
- [Number in College](https://studentaid.gov/2526/help/number-in-college)
- [Dependency Status](https://studentaid.gov/help-center/answers/article/dependency-status)
- [Prior Year Definition](https://studentaid.gov/2324/help/family-size)
- [FAFSA Glossary](https://studentaid.gov/help-center/answers/topic/glossary)

### Documentation
- **ENHANCEMENT-PLAN.md**: Full technical roadmap
- **IMPLEMENTATION-SUMMARY.md**: Detailed changelog
- **QUICK-START-GUIDE.md**: Implementation instructions

---

## 🎓 Educational Impact

### Success Metrics

**Quantitative Goals:**
- ⬇️ Reduce FAFSA household size errors by 50%
- ⬆️ Achieve 95%+ worksheet completion rate
- ⬆️ Increase time spent on educational content
- ⬆️ Knowledge check pass rates improve over time

**Qualitative Goals:**
- Students understand the 51% support rule
- Fewer questions to financial aid counselors
- Increased confidence in completing FAFSA
- Positive student feedback on clarity

---

## 🔄 Maintenance

### Annual Updates Required
- **Academic year options** (add new year, remove oldest)
- **FAFSA rule changes** (review federal student aid updates)
- **Tax year calculations** (verify prior-prior year formula)
- **Official links** (ensure StudentAid.gov URLs still work)

### Recommended Testing
- Test all tooltips (desktop + mobile)
- Verify running tally calculations
- Check knowledge quiz feedback
- Test PDF generation
- Validate across browsers
- Dark mode visual check

---

## 🤝 Contributing

We welcome contributions! Here's how:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Maintain MCF brand colors and styling
- Ensure mobile responsiveness
- Add tooltips for new FAFSA terms
- Keep auto-save functionality intact
- Test in all major browsers
- Update documentation

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🏆 Credits

**Developed by:** My College Finance (MCF)
**Version:** 2.0
**Last Updated:** November 3, 2025
**Total Development Time:** ~8 hours across 2 phases

**Special Thanks:**
- Google Gemini for enhancement recommendations
- FAFSA.gov for official guidance
- MCF students for user testing feedback

---

## 📚 Additional Documentation

For more detailed information, see:

- **[ENHANCEMENT-PLAN.md](ENHANCEMENT-PLAN.md)** - Complete feature roadmap with Phase 3-6 plans
- **[IMPLEMENTATION-SUMMARY.md](IMPLEMENTATION-SUMMARY.md)** - Detailed changelog of all enhancements
- **[QUICK-START-GUIDE.md](QUICK-START-GUIDE.md)** - Step-by-step implementation guide

---

## 💡 Pro Tips

### For Students
- ✅ Hover over EVERY blue ℹ️ icon - they contain valuable explanations
- ✅ Take the knowledge checks seriously - they prevent common mistakes
- ✅ Watch the running tally update - it helps you understand the calculations
- ✅ Use the Resource Hub links to verify information with official sources
- ✅ Download the PDF before closing - your data will be there next time, but backup is good!

### For Counselors
- ✅ Recommend students complete this BEFORE starting FAFSA
- ✅ Use the worksheet as a teaching tool in financial aid workshops
- ✅ Review the quiz questions with students who struggle
- ✅ Keep the PDF template for in-person counseling sessions

---

## 🎉 Success Stories

> *"I finally understand the 51% rule! This tool explained it better than any counselor."*
> — Student, Fall 2025

> *"The running tally made me realize I was counting my grandma wrong. Saved me from making a FAFSA error!"*
> — Student, Spring 2025

> *"As a financial aid counselor, this has cut down on household size questions by at least half."*
> — Financial Aid Counselor, MCF

---

## 📞 Support

For questions or support, please contact:

**[My College Finance Technical Feedback Form](https://forms.gle/your-form-id)**

---

## 📜 License

© 2025 My College Finance. All rights reserved.

---

## 🙏 Acknowledgments

**Created by:** [Thiink Media Graphics](https://thiinkmediagraphics.com)

**In partnership with:** [My College Finance](https://mycollegefinance.org)

---

## 🔗 Related Resources

- [FAFSA Interactive Research Web Report](https://studentaid.gov/data-center/student/application-volume/fafsa-completion-high-school)
- [My College Finance Main Website](https://mycollegefinance.org)
- [FAFSA Official Website](https://studentaid.gov/h/apply-for-aid/fafsa)
- [StudentAid.gov - Make FAFSA Corrections](https://studentaid.gov/apply-for-aid/fafsa/review-and-correct)

---

**🚀 Ready to get started? Open `index.html` and begin your FAFSA journey!**
