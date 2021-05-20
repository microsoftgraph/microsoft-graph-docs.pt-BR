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
# <a name="localizing-the-microsoft-graph-toolkit-components"></a><span data-ttu-id="8bb27-103">Localizando os componentes Graph Toolkit Microsoft</span><span class="sxs-lookup"><span data-stu-id="8bb27-103">Localizing the Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="8bb27-104">A localização é um aspecto importante do desenvolvimento de aplicativos para dar suporte a usuários com vários requisitos de idioma globalmente.</span><span class="sxs-lookup"><span data-stu-id="8bb27-104">Localization is an important aspect of application development to support users with various language requirements globally.</span></span>

<span data-ttu-id="8bb27-105">Você pode localizar os componentes Graph Toolkit microsoft para garantir que a interface do usuário reflita o idioma de destino.</span><span class="sxs-lookup"><span data-stu-id="8bb27-105">You can localize the Microsoft Graph Toolkit components to ensure that the UI reflects the target language.</span></span>

## <a name="use-localizationhelper-to-add-localized-strings"></a><span data-ttu-id="8bb27-106">Use LocalizationHelper para adicionar cadeias de caracteres localizadas</span><span class="sxs-lookup"><span data-stu-id="8bb27-106">Use LocalizationHelper to add localized strings</span></span>

<span data-ttu-id="8bb27-107">Nenhuma das cadeias de caracteres no kit de ferramentas está localizada, mas você pode fornecer suas próprias cadeias de caracteres localizadas e gerenciar idiomas diferentes por meio do mesmo processo usado para a localização do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8bb27-107">None of the strings in the toolkit are localized, but you can provide your own localized strings and manage different languages through the same process you use for localizing your app.</span></span> <span data-ttu-id="8bb27-108">Para facilitar a localização, o kit de ferramentas expõe a `LocalizationHelper` classe estática.</span><span class="sxs-lookup"><span data-stu-id="8bb27-108">To facilitate localization, the toolkit exposes the `LocalizationHelper` static class.</span></span>

<span data-ttu-id="8bb27-109">O exemplo a seguir mostra como localizar vários componentes.</span><span class="sxs-lookup"><span data-stu-id="8bb27-109">The following example shows how to localize several components.</span></span>

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

<span data-ttu-id="8bb27-110">Quando a propriedade de é atribuída, todos os componentes automaticamente pegarão as novas cadeias de caracteres e renderizarão, permitindo que você `strings` `LocalizationHelper` altere cadeias de caracteres dinamicamente.</span><span class="sxs-lookup"><span data-stu-id="8bb27-110">When the `strings` property of `LocalizationHelper` is assigned, all components will automatically pick up the new strings and re-render, allowing you to change strings dynamically.</span></span> 

<span data-ttu-id="8bb27-111">As cadeias de caracteres podem ser definidas em nível global ou por componente (com a `_components:` propriedade).</span><span class="sxs-lookup"><span data-stu-id="8bb27-111">The strings can be set at a global level or per component (with the `_components:` property).</span></span>

## <a name="strings"></a><span data-ttu-id="8bb27-112">Cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bb27-112">Strings</span></span>

### <a name="login"></a><span data-ttu-id="8bb27-113">Logon</span><span class="sxs-lookup"><span data-stu-id="8bb27-113">Login</span></span>

```ts
"login": {
  signInLinkSubtitle: "Sign In",
  signOutLinkSubtitle: "Sign Out"
}
```

### <a name="people-picker"></a><span data-ttu-id="8bb27-114">Seletor de Pessoas</span><span class="sxs-lookup"><span data-stu-id="8bb27-114">People-Picker</span></span>

```ts
"people-picker": {
  inputPlaceholderText: "Start typing a name",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="teams-channel-picker"></a><span data-ttu-id="8bb27-115">Teams-Channel-Picker</span><span class="sxs-lookup"><span data-stu-id="8bb27-115">Teams-Channel-Picker</span></span>

```ts
"teams-channel-picker": {
  inputPlaceholderText: "Select a channel",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="tasks"></a><span data-ttu-id="8bb27-116">Tarefas</span><span class="sxs-lookup"><span data-stu-id="8bb27-116">Tasks</span></span>

```ts
"tasks": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="tasks-base"></a><span data-ttu-id="8bb27-117">Tasks-Base</span><span class="sxs-lookup"><span data-stu-id="8bb27-117">Tasks-Base</span></span>

```ts
"tasks-base": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="todo"></a><span data-ttu-id="8bb27-118">Todo</span><span class="sxs-lookup"><span data-stu-id="8bb27-118">Todo</span></span>

```ts
"todo": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="person-card"></a><span data-ttu-id="8bb27-119">Cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="8bb27-119">Person-Card</span></span>

```ts
"person-card": {
  sendEmailLinkSubtitle: "Send email",
  startChatLinkSubtitle: "Start chat",
  showMoreSectionButton: "Show more"
}
```

### <a name="person-card-contact"></a><span data-ttu-id="8bb27-120">Person-Card-Contact</span><span class="sxs-lookup"><span data-stu-id="8bb27-120">Person-Card-Contact</span></span>

```ts
"person-card-contact": {
  contactSectionTitle: "Contact"
}
```

### <a name="person-card-organization"></a><span data-ttu-id="8bb27-121">Person-Card-Organization</span><span class="sxs-lookup"><span data-stu-id="8bb27-121">Person-Card-Organization</span></span>

```ts
"person-card-organization": {
  reportsToSectionTitle: "Reports to",
  directReportsSectionTitle: "Direct reports",
  organizationSectionTitle: "Organization",
  youWorkWithSubSectionTitle: "You work with",
  userWorksWithSubSectionTitle: "works with"
}
```

### <a name="person-card-messages"></a><span data-ttu-id="8bb27-122">Person-Card-Messages</span><span class="sxs-lookup"><span data-stu-id="8bb27-122">Person-Card-Messages</span></span>

```ts
"person-card-messages": {
  emailsSectionTitle: "Emails"
}
```

### <a name="person-card-files"></a><span data-ttu-id="8bb27-123">Person-Card-Files</span><span class="sxs-lookup"><span data-stu-id="8bb27-123">Person-Card-Files</span></span>

```ts
"person-card-files": {
  filesSectionTitle: "Files",
  sharedTextSubtitle: "Shared"
}
```

### <a name="person-card-profile"></a><span data-ttu-id="8bb27-124">Person-Card-Profile</span><span class="sxs-lookup"><span data-stu-id="8bb27-124">Person-Card-Profile</span></span>

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

### <a name="file"></a><span data-ttu-id="8bb27-125">File</span><span class="sxs-lookup"><span data-stu-id="8bb27-125">File</span></span>

```ts
'file': {
  modifiedSubtitle: 'Modified',
  sizeSubtitle: 'Size'
};
```

### <a name="file-list"></a><span data-ttu-id="8bb27-126">File-List</span><span class="sxs-lookup"><span data-stu-id="8bb27-126">File-List</span></span>

```ts
"file-list": {
  showMoreSubtitle: 'Show more items'
}
```
