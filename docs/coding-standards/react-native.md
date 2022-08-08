---
sidebar_position: 2
---

# REACT NATIVE

**Table of contents**:

- **Code Structure**
- **Structuring the folder**
- **Basics**
- **Naming Conventions**
- **Avoid Inline Stylings**
- **Do Use Safe Area View**
- **Do Use Keyboard Avoiding View**
- **Always Use loaders while fetching the data from API**
- **Bug Avoidance**
- **Environment Variables**
- **React Components**

## CODE STRUCTURE

Put all your imports in order at the very top of the code file. You shall ideally prioritize as follows:

```
import React from 'react';
import PropTypes from 'prop-types';
import {useTheme} from 'styled-components';
// Components
import {Picture} from '../';
// Icons
import {GreaterThan} from '../../assets/icons';
// Styled Components
import {
 Row,
 H5,
 SubTitle,
 BulletIn,
 HorizontalSpacer,
 Caption,
} from '../../assets/styles';
import {CardContainer, PatientDetailContainer, StatusContainer} from './styles';
// Utils
import normalize from '../../utils/pixelDensityHandler';
```

Ensure all your imports statements are on new lines, making your imports clean and easy to understand for all the components, third-party libraries, etc. Treat props as read-only. Do not try to modify them. 

2. Use index.js for each folder to export so that all the imports are referenced on the index.js file, and you don't have to write import statements again and again for every file. 	

