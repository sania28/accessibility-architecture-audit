[accessibility-report.md](https://github.com/user-attachments/files/32507658/accessibility-report.md)
# Accessibility Audit Report

## 1. Audit scope

The public W3C homepage was selected for the baseline accessibility audit:

https://www.w3.org/

Audit date: 21 September 2026

Tool: Lighthouse 13.4.1  
Browser engine: Chromium 153.0.0.0

## 2. Lighthouse result

The Lighthouse accessibility score was **100/100**.

The automated accessibility checks passed in the captured run. Lighthouse also listed several checks that require manual review, so the score is treated as a baseline rather than a complete accessibility certification.

## 3. Keyboard-only check

The page was checked without using the mouse.

Steps:
- Used `Tab` to move through interactive elements.
- Used `Shift + Tab` to move backwards.
- Used `Enter` on available links.
- Checked the visible focus movement.
- Checked whether focus became trapped.

### Result

No blocking keyboard navigation issue was found during the test.

## 4. Findings

The findings below are not presented as failed Lighthouse checks. They are areas to keep under review during future development.

### WEB-001 - Keyboard navigation

**Area:** Homepage navigation  
**WCAG:** 2.1.1 Keyboard  
**Priority:** Low

The keyboard pass worked without a blocking issue. The main concern is regression if navigation is changed later.

**Recommended fix:** Keep visible focus styles and include keyboard navigation in UI regression checks.

### WEB-002 - Interactive control naming

**Area:** Interactive controls  
**WCAG:** 4.1.2 Name, Role, Value  
**Priority:** Low

Lighthouse passed the accessible-name checks in this run. Any new custom control should follow the same pattern.

**Recommended fix:** Prefer native HTML controls and give custom controls clear accessible names and states.

### WEB-003 - Semantic content structure

**Area:** Main content and headings  
**WCAG:** 1.3.1 Info and Relationships  
**Priority:** Low

Lighthouse passed the main-landmark and heading-order checks. The semantic structure should remain consistent when content is extended.

**Recommended fix:** Keep a clear main region and use headings according to the content hierarchy.

### WEB-004 - Focus order

**Area:** Navigation and interactive content  
**WCAG:** 2.4.3 Focus Order  
**Priority:** Low

No incorrect focus order was noticed during the manual pass. DOM order should continue to match the intended interaction order.

**Recommended fix:** Avoid DOM or CSS changes that create a focus sequence different from the intended reading and interaction order.

### WEB-005 - Repository architecture

**Area:** Project structure  
**Reference:** Architecture / maintainability  
**Priority:** Medium

The project skeleton separates client, server, documentation and tests. These boundaries will make the later implementation easier to maintain.

**Recommended fix:** Keep each responsibility in its own top-level folder and add feature code inside the appropriate boundary.

## 5. Conclusion

The current Lighthouse result is 100/100 and the keyboard check did not show a blocking problem. The purpose of this audit is to establish a baseline and make accessibility checks part of future development.

The repository structure also provides a clean starting point for the next RabTech tasks involving semantic HTML, responsive CSS, JavaScript/API logic and the final capstone.
