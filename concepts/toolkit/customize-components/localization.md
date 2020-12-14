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
# <a name="localizing-the-microsoft-graph-toolkit-components"></a><span data-ttu-id="d64b0-103">Localizar os componentes do Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d64b0-103">Localizing the Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="d64b0-104">A localização é um aspecto importante do desenvolvimento de aplicativos para dar suporte a usuários com vários requisitos de idioma globalmente.</span><span class="sxs-lookup"><span data-stu-id="d64b0-104">Localization is a important aspect of application development to support users with various language requirements globally.</span></span>

<span data-ttu-id="d64b0-105">Você pode localizar os componentes do kit de ferramentas do Microsoft Graph para garantir que a interface do usuário reflita o idioma de destino.</span><span class="sxs-lookup"><span data-stu-id="d64b0-105">You can localize the Microsoft Graph Toolkit components to ensure that the UI reflects the target language.</span></span>

## <a name="use-localizationhelper-to-add-localized-strings"></a><span data-ttu-id="d64b0-106">Usar LocalizationHelper para adicionar cadeias de caracteres localizadas</span><span class="sxs-lookup"><span data-stu-id="d64b0-106">Use LocalizationHelper to add localized strings</span></span>

<span data-ttu-id="d64b0-107">Todas as cadeias de caracteres no kit de ferramentas não são localizadas, mas você pode fornecer suas próprias cadeias de caracteres localizadas e gerenciar idiomas diferentes pelo mesmo processo que você usa para localizar seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d64b0-107">All strings in the toolkit are not localized, but you can provide your own localized strings and manage different languages through the same process you use for localizing your app.</span></span> <span data-ttu-id="d64b0-108">Para facilitar a localização, o kit de ferramentas expõe a `LocalizationHelper` classe estática.</span><span class="sxs-lookup"><span data-stu-id="d64b0-108">To facilitate localization, the toolkit exposes the `LocalizationHelper` static class.</span></span>

<span data-ttu-id="d64b0-109">O exemplo a seguir mostra como localizar vários componentes.</span><span class="sxs-lookup"><span data-stu-id="d64b0-109">The following example shows how to localize several components.</span></span>

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

<span data-ttu-id="d64b0-110">Quando a `strings` propriedade for atribuída, todos os componentes selecionarão automaticamente as novas cadeias de caracteres e serão renderizados novamente, permitindo que você altere as cadeias de caracteres dinamicamente.</span><span class="sxs-lookup"><span data-stu-id="d64b0-110">When the `strings` property is assigned, all components will automatically pick up the new strings and re-render, allowing you to change strings dynamically.</span></span> 

<span data-ttu-id="d64b0-111">As cadeias de caracteres podem ser definidas em um nível global ou por componente (com a `_components:` Propriedade).</span><span class="sxs-lookup"><span data-stu-id="d64b0-111">The strings can be set at a global level or per component (with the `_components:` property).</span></span>

## <a name="strings"></a><span data-ttu-id="d64b0-112">Cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d64b0-112">Strings</span></span>

### <a name="login"></a><span data-ttu-id="d64b0-113">Logon</span><span class="sxs-lookup"><span data-stu-id="d64b0-113">Login</span></span>

```ts
{
  signInLinkSubtitle: 'Sign In',
  signOutLinkSubtitle: 'Sign Out'
}
```

### <a name="people-picker"></a><span data-ttu-id="d64b0-114">Seletor de Pessoas</span><span class="sxs-lookup"><span data-stu-id="d64b0-114">People-Picker</span></span>

```ts
{
  inputPlaceholderText: 'Start typing a name',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="teams-channel-picker"></a><span data-ttu-id="d64b0-115">Teams – seletor de canal</span><span class="sxs-lookup"><span data-stu-id="d64b0-115">Teams-Channel-Picker</span></span>

```ts
{
  inputPlaceholderText: 'Select a channel',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="tasks"></a><span data-ttu-id="d64b0-116">Tarefas</span><span class="sxs-lookup"><span data-stu-id="d64b0-116">Tasks</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="tasks-base"></a><span data-ttu-id="d64b0-117">Tasks-Base</span><span class="sxs-lookup"><span data-stu-id="d64b0-117">Tasks-Base</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="todo"></a><span data-ttu-id="d64b0-118">Fazer</span><span class="sxs-lookup"><span data-stu-id="d64b0-118">Todo</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="person-card"></a><span data-ttu-id="d64b0-119">Cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="d64b0-119">Person-Card</span></span>

```ts
{
  sendEmailLinkSubtitle: 'Send email',
  startChatLinkSubtitle: 'Start chat',
  showMoreSectionButton: 'Show more'
}
```

### <a name="person-card-contact"></a><span data-ttu-id="d64b0-120">Pessoa-cartão-contato</span><span class="sxs-lookup"><span data-stu-id="d64b0-120">Person-Card-Contact</span></span>

```ts
{
  contactSectionTitle: "Contact";
}
```

### <a name="person-card-organization"></a><span data-ttu-id="d64b0-121">Pessoa-cartão-organização</span><span class="sxs-lookup"><span data-stu-id="d64b0-121">Person-Card-Organization</span></span>

```ts
{
  reportsToSectionTitle: 'Reports to',
  directReportsSectionTitle: 'Direct reports',
  organizationSectionTitle: 'Organization',
  youWorkWithSubSectionTitle: 'You work with',
  userWorksWithSubSectionTitle: 'works with'
}
```

### <a name="person-card-messages"></a><span data-ttu-id="d64b0-122">Pessoa-cartão-mensagens</span><span class="sxs-lookup"><span data-stu-id="d64b0-122">Person-Card-Messages</span></span>

```ts
{
  emailsSectionTitle: "Emails";
}
```

### <a name="person-card-files"></a><span data-ttu-id="d64b0-123">Pessoa-cartão-arquivos</span><span class="sxs-lookup"><span data-stu-id="d64b0-123">Person-Card-Files</span></span>

```ts
{
  filesSectionTitle: 'Files',
  sharedTextSubtitle: 'Shared'
}
```

### <a name="person-card-profile"></a><span data-ttu-id="d64b0-124">Person-Card-Profile</span><span class="sxs-lookup"><span data-stu-id="d64b0-124">Person-Card-Profile</span></span>

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
