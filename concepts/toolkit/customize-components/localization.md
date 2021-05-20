---
title: Localizando os componentes Graph Toolkit Microsoft
description: Use LocalizationHelper para localização dos componentes Graph Toolkit Microsoft.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: d333112e77d047151aa6b030acd0ed1cea626573
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579925"
---
# <a name="localizing-the-microsoft-graph-toolkit-components"></a>Localizando os componentes Graph Toolkit Microsoft

A localização é um aspecto importante do desenvolvimento de aplicativos para dar suporte a usuários com vários requisitos de idioma globalmente.

Você pode localizar os componentes Graph Toolkit microsoft para garantir que a interface do usuário reflita o idioma de destino.

## <a name="use-localizationhelper-to-add-localized-strings"></a>Use LocalizationHelper para adicionar cadeias de caracteres localizadas

Nenhuma das cadeias de caracteres no kit de ferramentas está localizada, mas você pode fornecer suas próprias cadeias de caracteres localizadas e gerenciar idiomas diferentes por meio do mesmo processo usado para a localização do aplicativo. Para facilitar a localização, o kit de ferramentas expõe a `LocalizationHelper` classe estática.

O exemplo a seguir mostra como localizar vários componentes.

```ts
import { LocalizationHelper } from "@microsoft/mgt";

LocalizationHelper.strings = {
  noResultsFound: "لم نجد أي قنوات",
  _components: {
    "login": {
      signInLinkSubtitle: "login",
      signOutLinkSubtitle: "خروج",
    },
    "people-picker": {
      inputPlaceholderText: "ابدأ في كتابة الاسم",
      noResultsFound: "لم نجد أي قنوات", // will overwrite globally defined noResultsFound in people-picker component
      loadingMessage: "...جار التحميل",
    },
    "teams-channel-picker": {
      inputPlaceholderText: "حدد قناة",
      noResultsFound: "local NoResultsFound Example",
      // loadingMessage: is default string "Loading..." for this example since not defined globally or locally
    },
    "tasks": {
      removeTaskSubtitle: "delete",
      cancelNewTaskSubtitle: "canceltest",
      newTaskPlaceholder: "newTaskTest",
      addTaskButtonSubtitle: "addme",
    },
    "person-card": {
      sendEmailLinkSubtitle: "ارسل بريد الكتروني",
      startChatLinkSubtitle: "ابدأ الدردشة",
      showExpandedDetailsButton: 'Show expanded details',
      showMoreSectionButton: "أظهر المزيد", // global declaration
    },
    "person-card-contact": {
      contactSectionTitle: "اتصل",
    },
    "person-card-organization": {
      reportsToSectionTitle: "تقارير ل",
      directReportsSectionTitle: "تقارير مباشرة",
      organizationSectionTitle: "منظمة",
      youWorkWithSubSectionTitle: "انت تعمل مع",
      userWorksWithSubSectionTitle: "يعمل مع",
    },
  },
};
```

Quando a propriedade de é atribuída, todos os componentes automaticamente pegarão as novas cadeias de caracteres e renderizarão, permitindo que você `strings` `LocalizationHelper` altere cadeias de caracteres dinamicamente. 

As cadeias de caracteres podem ser definidas em nível global ou por componente (com a `_components:` propriedade).

## <a name="strings"></a>Cadeias de caracteres

### <a name="login"></a>Logon

```ts
"login": {
  signInLinkSubtitle: "Sign In",
  signOutLinkSubtitle: "Sign Out"
}
```

### <a name="people-picker"></a>Seletor de Pessoas

```ts
"people-picker": {
  inputPlaceholderText: "Start typing a name",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="teams-channel-picker"></a>Teams-Channel-Picker

```ts
"teams-channel-picker": {
  inputPlaceholderText: "Select a channel",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="tasks"></a>Tarefas

```ts
"tasks": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="tasks-base"></a>Tasks-Base

```ts
"tasks-base": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="todo"></a>Todo

```ts
"todo": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="person-card"></a>Cartão de pessoa

```ts
"person-card": {
  sendEmailLinkSubtitle: "Send email",
  startChatLinkSubtitle: "Start chat",
  showMoreSectionButton: "Show more"
}
```

### <a name="person-card-contact"></a>Person-Card-Contact

```ts
"person-card-contact": {
  contactSectionTitle: "Contact"
}
```

### <a name="person-card-organization"></a>Person-Card-Organization

```ts
"person-card-organization": {
  reportsToSectionTitle: "Reports to",
  directReportsSectionTitle: "Direct reports",
  organizationSectionTitle: "Organization",
  youWorkWithSubSectionTitle: "You work with",
  userWorksWithSubSectionTitle: "works with"
}
```

### <a name="person-card-messages"></a>Person-Card-Messages

```ts
"person-card-messages": {
  emailsSectionTitle: "Emails"
}
```

### <a name="person-card-files"></a>Person-Card-Files

```ts
"person-card-files": {
  filesSectionTitle: "Files",
  sharedTextSubtitle: "Shared"
}
```

### <a name="person-card-profile"></a>Person-Card-Profile

```ts
"person-card-profile": {
  SkillsAndExperienceSectionTitle: "Skills & Experience",
  AboutCompactSectionTitle: "About",
  SkillsSubSectionTitle: "Skills",
  LanguagesSubSectionTitle: "Languages",
  WorkExperienceSubSectionTitle: "Work Experience",
  EducationSubSectionTitle: "Education",
  professionalInterestsSubSectionTitle: "Professional Interests",
  personalInterestsSubSectionTitle: "Personal Interests",
  birthdaySubSectionTitle: "Birthday",
  currentYearSubtitle: "Current"
}
```

### <a name="file"></a>File

```ts
'file': {
  modifiedSubtitle: 'Modified',
  sizeSubtitle: 'Size'
};
```

### <a name="file-list"></a>File-List

```ts
"file-list": {
  showMoreSubtitle: 'Show more items'
}
```
