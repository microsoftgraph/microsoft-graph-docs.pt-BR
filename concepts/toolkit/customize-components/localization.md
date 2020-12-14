---
title: Localizar os componentes do Microsoft Graph Toolkit
description: Use o LocalizationHelper para localizar os componentes do Microsoft Graph Toolkit.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 3ac9f3fe5dedeb4e1793a589778242486f3b0070
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660090"
---
# <a name="localizing-the-microsoft-graph-toolkit-components"></a>Localizar os componentes do Microsoft Graph Toolkit

A localização é um aspecto importante do desenvolvimento de aplicativos para dar suporte a usuários com vários requisitos de idioma globalmente.

Você pode localizar os componentes do kit de ferramentas do Microsoft Graph para garantir que a interface do usuário reflita o idioma de destino.

## <a name="use-localizationhelper-to-add-localized-strings"></a>Usar LocalizationHelper para adicionar cadeias de caracteres localizadas

Todas as cadeias de caracteres no kit de ferramentas não são localizadas, mas você pode fornecer suas próprias cadeias de caracteres localizadas e gerenciar idiomas diferentes pelo mesmo processo que você usa para localizar seu aplicativo. Para facilitar a localização, o kit de ferramentas expõe a `LocalizationHelper` classe estática.

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
      noResultsFound: "لم نجد أي قنوات", //collision with global defined noResultsFound will overwrite with local result
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

Quando a `strings` propriedade for atribuída, todos os componentes selecionarão automaticamente as novas cadeias de caracteres e serão renderizados novamente, permitindo que você altere as cadeias de caracteres dinamicamente. 

As cadeias de caracteres podem ser definidas em um nível global ou por componente (com a `_components:` Propriedade).

## <a name="strings"></a>Cadeias de caracteres

### <a name="login"></a>Logon

```ts
{
  signInLinkSubtitle: 'Sign In',
  signOutLinkSubtitle: 'Sign Out'
}
```

### <a name="people-picker"></a>Seletor de Pessoas

```ts
{
  inputPlaceholderText: 'Start typing a name',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="teams-channel-picker"></a>Teams – seletor de canal

```ts
{
  inputPlaceholderText: 'Select a channel',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="tasks"></a>Tarefas

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="tasks-base"></a>Tasks-Base

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="todo"></a>Fazer

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="person-card"></a>Cartão de pessoa

```ts
{
  sendEmailLinkSubtitle: 'Send email',
  startChatLinkSubtitle: 'Start chat',
  showMoreSectionButton: 'Show more'
}
```

### <a name="person-card-contact"></a>Pessoa-cartão-contato

```ts
{
  contactSectionTitle: "Contact";
}
```

### <a name="person-card-organization"></a>Pessoa-cartão-organização

```ts
{
  reportsToSectionTitle: 'Reports to',
  directReportsSectionTitle: 'Direct reports',
  organizationSectionTitle: 'Organization',
  youWorkWithSubSectionTitle: 'You work with',
  userWorksWithSubSectionTitle: 'works with'
}
```

### <a name="person-card-messages"></a>Pessoa-cartão-mensagens

```ts
{
  emailsSectionTitle: "Emails";
}
```

### <a name="person-card-files"></a>Pessoa-cartão-arquivos

```ts
{
  filesSectionTitle: 'Files',
  sharedTextSubtitle: 'Shared'
}
```

### <a name="person-card-profile"></a>Person-Card-Profile

```ts
{
  SkillsAndExperienceSectionTitle: 'Skills & Experience',
  AboutCompactSectionTitle: 'About',
  SkillsSubSectionTitle: 'Skills',
  LanguagesSubSectionTitle: 'Languages',
  WorkExperienceSubSectionTitle: 'Work Experience',
  EducationSubSectionTitle: 'Education',
  professionalInterestsSubSectionTitle: 'Professional Interests',
  personalInterestsSubSectionTitle: 'Personal Interests',
  birthdaySubSectionTitle: 'Birthday',
  currentYearSubtitle: 'Current'
}
```
