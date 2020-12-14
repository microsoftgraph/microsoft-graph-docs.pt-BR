---
title: Person-Card componente no kit de ferramentas do Microsoft Graph
description: Um componente de Person-Card é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 79a14c3d37fba06a076e319b34029008b7fbf2fd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659180"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="7af8d-103">Person-Card componente no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7af8d-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="7af8d-104">Um componente de Person-Card é um componente responsivo para exibir mais informações relacionadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="7af8d-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="7af8d-105">Geralmente, é usado como um submenu do `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="7af8d-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="7af8d-106">Para obter mais informações sobre o `mgt-person` componente, consulte [Gerenciamento-pessoa](./person.md).</span><span class="sxs-lookup"><span data-stu-id="7af8d-106">For more information about the `mgt-person` component, see [mgt-person](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="7af8d-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7af8d-107">Example</span></span>

<span data-ttu-id="7af8d-108">O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="7af8d-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="7af8d-109">Passe o mouse sobre a pessoa para ver o cartão Person e use o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="7af8d-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="7af8d-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="7af8d-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a><span data-ttu-id="7af8d-111">Configuração de componente global</span><span class="sxs-lookup"><span data-stu-id="7af8d-111">Global component configuration</span></span>

<span data-ttu-id="7af8d-112">A `MgtPersonCard` classe expõe um `config` objeto estático que configura todos os componentes de cartão de pessoa no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7af8d-112">The `MgtPersonCard` class exposes a static `config` object that configures all person card components in the application.</span></span> <span data-ttu-id="7af8d-113">O objeto config Configura quais seções e quais APIs são usadas pelo cartão de pessoa para buscar detalhes sobre um usuário do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7af8d-113">The config object configures what sections and what APIs are used by the person card to fetch details about a user from Microsoft Graph.</span></span>

<span data-ttu-id="7af8d-114">Por padrão, todas as seções e APIs estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="7af8d-114">By default, all sections and APIs are enabled.</span></span> <span data-ttu-id="7af8d-115">O exemplo a seguir mostra como usar o objeto config para desabilitar seções ou APIs.</span><span class="sxs-lookup"><span data-stu-id="7af8d-115">The following example shows how to use the config object to disable sections or APIs.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

<span data-ttu-id="7af8d-116">As propriedades a seguir estão disponíveis no objeto config.</span><span class="sxs-lookup"><span data-stu-id="7af8d-116">The following properties are available on the config object.</span></span>

| <span data-ttu-id="7af8d-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7af8d-117">Property</span></span> | <span data-ttu-id="7af8d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7af8d-118">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="7af8d-119">useContactApis</span><span class="sxs-lookup"><span data-stu-id="7af8d-119">useContactApis</span></span> | <span data-ttu-id="7af8d-120">`boolean` – Indica se o componente de cartão de pessoa pode usar a API de contato do Microsoft Graph para pesquisar detalhes e fotos de contato.</span><span class="sxs-lookup"><span data-stu-id="7af8d-120">`boolean` - Indicates whether the person card component can use the Microsoft Graph Contact API to search for contact details and photos.</span></span> <span data-ttu-id="7af8d-121">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7af8d-121">Default value is `true`.</span></span>  |
| <span data-ttu-id="7af8d-122">seções</span><span class="sxs-lookup"><span data-stu-id="7af8d-122">sections</span></span> | <span data-ttu-id="7af8d-123">`object` -Configura quais seções são mostradas no cartão de pessoa.</span><span class="sxs-lookup"><span data-stu-id="7af8d-123">`object` - Configures what sections are shown in the person card.</span></span>  |

### <a name="person-card-sections"></a><span data-ttu-id="7af8d-124">Seções de cartões de pessoa</span><span class="sxs-lookup"><span data-stu-id="7af8d-124">Person card sections</span></span>

<span data-ttu-id="7af8d-125">O cartão de pessoa contém várias seções configuráveis para exibir os detalhes da pessoa:</span><span class="sxs-lookup"><span data-stu-id="7af8d-125">The person card contains several configurable sections for displaying person details:</span></span>
* <span data-ttu-id="7af8d-126">Contato – informações de contato, como email, telefone, cargo, local e muito mais.</span><span class="sxs-lookup"><span data-stu-id="7af8d-126">Contact - Contact information such as email, phone, position, location, and more.</span></span>
* <span data-ttu-id="7af8d-127">Organização-gráfico organizacional com gerentes, subordinados diretos e pessoas relevantes.</span><span class="sxs-lookup"><span data-stu-id="7af8d-127">Organization - Organizational graph with managers, direct reports, and relevant people.</span></span>
* <span data-ttu-id="7af8d-128">Mensagens – mensagens de email mais relevantes com o usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="7af8d-128">Messages - Most relevant email messages with the current signed in user.</span></span>
* <span data-ttu-id="7af8d-129">Arquivos-arquivos compartilhados mais relevantes com o usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="7af8d-129">Files - Most relevant shared files with the current signed in user.</span></span>
* <span data-ttu-id="7af8d-130">Profile-informações de perfil, como projetos, habilidades, idiomas e muito mais.</span><span class="sxs-lookup"><span data-stu-id="7af8d-130">Profile - Profile information such as projects, skills, languages, and more.</span></span>

<span data-ttu-id="7af8d-131">As seções são carregadas por padrão, mas podem ser desabilitadas globalmente por meio da `MgtPersonCard.config.sections` propriedade Object.</span><span class="sxs-lookup"><span data-stu-id="7af8d-131">Sections are loaded by default, but they can be disabled globally via the `MgtPersonCard.config.sections` object property.</span></span> <span data-ttu-id="7af8d-132">As propriedades a seguir estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7af8d-132">The following properties are available.</span></span>

| <span data-ttu-id="7af8d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7af8d-133">Property</span></span> | <span data-ttu-id="7af8d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="7af8d-134">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="7af8d-135">organization</span><span class="sxs-lookup"><span data-stu-id="7af8d-135">organization</span></span> | <span data-ttu-id="7af8d-136">`boolean` -Indica se a seção de organização de cartões de pessoa é exibida.</span><span class="sxs-lookup"><span data-stu-id="7af8d-136">`boolean` - Indicates whether the person card organization section is shown.</span></span> <span data-ttu-id="7af8d-137">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7af8d-137">Default value is `true`.</span></span>  |
| <span data-ttu-id="7af8d-138">mailMessage</span><span class="sxs-lookup"><span data-stu-id="7af8d-138">mailMessages</span></span> | <span data-ttu-id="7af8d-139">`boolean` -Indica se a seção mensagens de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="7af8d-139">`boolean` - Indicates whether the person card messages section is shown.</span></span> <span data-ttu-id="7af8d-140">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7af8d-140">Default value is `true`.</span></span>  |
| <span data-ttu-id="7af8d-141">arquivos</span><span class="sxs-lookup"><span data-stu-id="7af8d-141">files</span></span> | <span data-ttu-id="7af8d-142">`boolean` -Indica se a seção arquivos de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="7af8d-142">`boolean` - Indicates whether the person card files section is shown.</span></span> <span data-ttu-id="7af8d-143">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7af8d-143">Default value is `true`.</span></span>  |
| <span data-ttu-id="7af8d-144">perfil</span><span class="sxs-lookup"><span data-stu-id="7af8d-144">profile</span></span> | <span data-ttu-id="7af8d-145">`boolean` -Indica se a seção de perfil de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="7af8d-145">`boolean` - Indicates whether the person card profile section is shown.</span></span> <span data-ttu-id="7af8d-146">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7af8d-146">Default value is `true`.</span></span>  |

<span data-ttu-id="7af8d-147">Para desabilitar uma seção, basta definir a propriedade como `false` em seu código de inicialização do aplicativo:.</span><span class="sxs-lookup"><span data-stu-id="7af8d-147">To disable a section, simply set the property to `false` in your app initialization code:.</span></span>
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="7af8d-148">Configuração para integrações do teams</span><span class="sxs-lookup"><span data-stu-id="7af8d-148">Setup for Teams integrations</span></span>

<span data-ttu-id="7af8d-149">O componente Person-Card permite que o usuário entre em contato com a pessoa de destino, incluindo via chat do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7af8d-149">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="7af8d-150">Se estiver usando o componente dentro de um aplicativo de guia do Teams, você pode garantir que o componente se vincule diretamente a um chat, em vez de abrir uma janela do navegador, definindo o `microsoftTeamsLib` no `TeamsProvider` .</span><span class="sxs-lookup"><span data-stu-id="7af8d-150">If using the component inside a Teams tab app, you can ensure that the component deep links directly to a chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="7af8d-151">Se o componente de Person-Card não conseguir detectar a biblioteca do Teams, o componente tentará abrir o cliente da Web do teams.</span><span class="sxs-lookup"><span data-stu-id="7af8d-151">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

<span data-ttu-id="7af8d-152">Para obter mais informações sobre o `TeamsProvider` provedor, consulte [Microsoft Teams Provider](../providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="7af8d-152">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7af8d-153">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7af8d-153">Properties</span></span>

<span data-ttu-id="7af8d-154">Por padrão, o `mgt-person` componente passará os detalhes da pessoa para o `mgt-person-card` componente.</span><span class="sxs-lookup"><span data-stu-id="7af8d-154">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="7af8d-155">No entanto, você pode usar esses atributos para mudar isso ao padronizar o `mgt-person` componente ou ao usar o `mgt-person-card` componente como um componente autônomo.</span><span class="sxs-lookup"><span data-stu-id="7af8d-155">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="7af8d-156">Atributo</span><span class="sxs-lookup"><span data-stu-id="7af8d-156">Attribute</span></span>         | <span data-ttu-id="7af8d-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="7af8d-157">Type</span></span>                     | <span data-ttu-id="7af8d-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="7af8d-158">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="7af8d-159">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="7af8d-159">person-details</span></span> | <span data-ttu-id="7af8d-160">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="7af8d-160">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="7af8d-161">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="7af8d-161">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="7af8d-162">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="7af8d-162">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="7af8d-163">Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7af8d-163">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="7af8d-164">pessoa-imagem</span><span class="sxs-lookup"><span data-stu-id="7af8d-164">person-image</span></span>   | <span data-ttu-id="7af8d-165">string</span><span class="sxs-lookup"><span data-stu-id="7af8d-165">string</span></span>                    | <span data-ttu-id="7af8d-166">URI de imagem relacionado à pessoa exibida no cartão.</span><span class="sxs-lookup"><span data-stu-id="7af8d-166">Image uri related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="7af8d-167">Inherit-detalhes</span><span class="sxs-lookup"><span data-stu-id="7af8d-167">inherit-details</span></span>   | <span data-ttu-id="7af8d-168">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7af8d-168">None.</span></span>                  | <span data-ttu-id="7af8d-169">Permite que o cartão de pessoa percorra a árvore pai para `mgt-person` que o componente use o mesmo `person-details` e os `person-image` dados.</span><span class="sxs-lookup"><span data-stu-id="7af8d-169">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="7af8d-170">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="7af8d-170">user-id</span></span> | <span data-ttu-id="7af8d-171">string</span><span class="sxs-lookup"><span data-stu-id="7af8d-171">string</span></span> | <span data-ttu-id="7af8d-172">Permite que os desenvolvedores forneçam o ID de usuário para dados de recuperar exibidos no componente de cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="7af8d-172">Allows developers to supply user-id to retrive data shown on person-card component</span></span> |
| <span data-ttu-id="7af8d-173">pessoa – consulta</span><span class="sxs-lookup"><span data-stu-id="7af8d-173">person-query</span></span> | <span data-ttu-id="7af8d-174">string</span><span class="sxs-lookup"><span data-stu-id="7af8d-174">string</span></span> | <span data-ttu-id="7af8d-175">Permite que os desenvolvedores forneçam uma consulta de pessoa para dados de recuperar exibidos no componente de cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="7af8d-175">Allows developers to supply person-query to retrive data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="7af8d-176">Modelos</span><span class="sxs-lookup"><span data-stu-id="7af8d-176">Templates</span></span>

<span data-ttu-id="7af8d-177">O componente Person-Card usa [modelos](../customize-components/templates.md) que permitem que você adicione ou substitua partes do componente.</span><span class="sxs-lookup"><span data-stu-id="7af8d-177">The Person-Card component uses [templates](../customize-components/templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="7af8d-178">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="7af8d-178">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="7af8d-179">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="7af8d-179">Data type</span></span> | <span data-ttu-id="7af8d-180">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="7af8d-180">Data context</span></span> | <span data-ttu-id="7af8d-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="7af8d-181">Description</span></span> |
| - | - | - |
| <span data-ttu-id="7af8d-182">sem dados</span><span class="sxs-lookup"><span data-stu-id="7af8d-182">no-data</span></span> | <span data-ttu-id="7af8d-183">null</span><span class="sxs-lookup"><span data-stu-id="7af8d-183">null</span></span> | <span data-ttu-id="7af8d-184">O modelo usado quando não há dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7af8d-184">The template used when no data is available.</span></span>
| <span data-ttu-id="7af8d-185">Padrão.</span><span class="sxs-lookup"><span data-stu-id="7af8d-185">default</span></span> | <span data-ttu-id="7af8d-186">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="7af8d-186">`person`: The person details object</span></span> <br> <span data-ttu-id="7af8d-187">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="7af8d-187">`personImage`: The URL of the image</span></span> | <span data-ttu-id="7af8d-188">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="7af8d-188">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="7af8d-189">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="7af8d-189">person-details</span></span> | <span data-ttu-id="7af8d-190">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="7af8d-190">`person`: The person details object</span></span> | <span data-ttu-id="7af8d-191">O modelo usado para renderizar a parte superior do cartão Person.</span><span class="sxs-lookup"><span data-stu-id="7af8d-191">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="7af8d-192">adicional-detalhes</span><span class="sxs-lookup"><span data-stu-id="7af8d-192">additional-details</span></span> | <span data-ttu-id="7af8d-193">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="7af8d-193">`person`: The person details object</span></span> <br> <span data-ttu-id="7af8d-194">`personImage`: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="7af8d-194">`personImage`: the URL of the image</span></span> | <span data-ttu-id="7af8d-195">O modelo usado para adicionar conteúdo personalizado ao contêiner detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="7af8d-195">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="7af8d-196">Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão.</span><span class="sxs-lookup"><span data-stu-id="7af8d-196">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" view="twolines" person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="css-custom-properties"></a><span data-ttu-id="7af8d-197">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="7af8d-197">CSS custom properties</span></span>

<span data-ttu-id="7af8d-198">O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="7af8d-198">The `mgt-person-card` component defines the following CSS custom properties.</span></span> 

```css
mgt-person {
  --person-card-display-name-font-size: 40px;
  --person-card-display-name-color: #ffffff;
  --person-card-title-font-size: 20px;
  --person-card-title-color: #ffffff;
  --person-card-subtitle-font-size: 10px;
  --person-card-subtitle-color: #ffffff;
  --person-card-details-title-font-size: 10px;
  --person-card-details-title-color: #b3bf0a;
  --person-card-details-item-font-size: 20px;
  --person-card-details-item-color: #3abf0a;
  --person-card-background-color: #000000;
}
```

<span data-ttu-id="7af8d-199">Para saber mais, confira [estilos de componentes](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="7af8d-199">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="7af8d-200">APIs e permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7af8d-200">Microsoft Graph APIs and permissions</span></span>

<span data-ttu-id="7af8d-201">O controle Person-Card usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7af8d-201">The Person-Card control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="7af8d-202">Recurso</span><span class="sxs-lookup"><span data-stu-id="7af8d-202">Resource</span></span> | <span data-ttu-id="7af8d-203">Permissão</span><span class="sxs-lookup"><span data-stu-id="7af8d-203">Permission</span></span> | <span data-ttu-id="7af8d-204">Seção</span><span class="sxs-lookup"><span data-stu-id="7af8d-204">Section</span></span> |
| - | - | - |
| [<span data-ttu-id="7af8d-205">/me</span><span class="sxs-lookup"><span data-stu-id="7af8d-205">/me</span></span>](/graph/api/user-get) | <span data-ttu-id="7af8d-206">User.Read</span><span class="sxs-lookup"><span data-stu-id="7af8d-206">User.Read</span></span> | <span data-ttu-id="7af8d-207">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-207">Default</span></span> |
| [<span data-ttu-id="7af8d-208">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="7af8d-208">/me/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="7af8d-209">User.Read</span><span class="sxs-lookup"><span data-stu-id="7af8d-209">User.Read</span></span> | <span data-ttu-id="7af8d-210">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-210">Default</span></span> |
| [<span data-ttu-id="7af8d-211">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="7af8d-211">/me/people/?$search=</span></span>](/graph/api/user-list-people) | <span data-ttu-id="7af8d-212">People.Read</span><span class="sxs-lookup"><span data-stu-id="7af8d-212">People.Read</span></span> | <span data-ttu-id="7af8d-213">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-213">Default</span></span> |
| [<span data-ttu-id="7af8d-214">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="7af8d-214">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="7af8d-215">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7af8d-215">Contacts.Read</span></span> | <span data-ttu-id="7af8d-216">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-216">Default</span></span> |
| [<span data-ttu-id="7af8d-217">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="7af8d-217">/users/{id}</span></span>](/graph/api/user-list-people) | <span data-ttu-id="7af8d-218">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-218">User.ReadBasic.All</span></span> | <span data-ttu-id="7af8d-219">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-219">Default</span></span> |
| [<span data-ttu-id="7af8d-220">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="7af8d-220">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="7af8d-221">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-221">User.ReadBasic.All</span></span> | <span data-ttu-id="7af8d-222">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-222">Default</span></span> |
| [<span data-ttu-id="7af8d-223">/me/presence</span><span class="sxs-lookup"><span data-stu-id="7af8d-223">/me/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="7af8d-224">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="7af8d-224">Presence.Read</span></span> | <span data-ttu-id="7af8d-225">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-225">Default</span></span> |
| [<span data-ttu-id="7af8d-226">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="7af8d-226">/users/{id}/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="7af8d-227">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-227">Presence.Read.All</span></span> | <span data-ttu-id="7af8d-228">Padrão</span><span class="sxs-lookup"><span data-stu-id="7af8d-228">Default</span></span> |
| [<span data-ttu-id="7af8d-229">/users/{id}/manager</span><span class="sxs-lookup"><span data-stu-id="7af8d-229">/users/{id}/manager</span></span>](/graph/api/user-list-manager) | <span data-ttu-id="7af8d-230">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-230">User.Read.All</span></span> | <span data-ttu-id="7af8d-231">Organização</span><span class="sxs-lookup"><span data-stu-id="7af8d-231">Organization</span></span> |
| [<span data-ttu-id="7af8d-232">/users/{id}/directReports</span><span class="sxs-lookup"><span data-stu-id="7af8d-232">/users/{id}/directReports</span></span>](/graph/api/user-list-directreports) | <span data-ttu-id="7af8d-233">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-233">User.Read.All</span></span> | <span data-ttu-id="7af8d-234">Organização</span><span class="sxs-lookup"><span data-stu-id="7af8d-234">Organization</span></span> |
| [<span data-ttu-id="7af8d-235">/users/{id}/people</span><span class="sxs-lookup"><span data-stu-id="7af8d-235">/users/{id}/people</span></span>](/graph/api/user-list-people) | <span data-ttu-id="7af8d-236">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-236">People.Read.All</span></span> | <span data-ttu-id="7af8d-237">Organização</span><span class="sxs-lookup"><span data-stu-id="7af8d-237">Organization</span></span> |
| [<span data-ttu-id="7af8d-238">/me/messages</span><span class="sxs-lookup"><span data-stu-id="7af8d-238">/me/messages</span></span>](/graph/api/user-list-messages) | <span data-ttu-id="7af8d-239">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="7af8d-239">Mail.ReadBasic</span></span> | <span data-ttu-id="7af8d-240">Mensagens</span><span class="sxs-lookup"><span data-stu-id="7af8d-240">Messages</span></span> |
| <span data-ttu-id="7af8d-241">[/me/insights/Shared](/graph/api/insights-list-shared) e [/me/insights/used](/graph/api/insights-list-used)</span><span class="sxs-lookup"><span data-stu-id="7af8d-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span></span> | <span data-ttu-id="7af8d-242">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-242">Sites.Read.All</span></span> | <span data-ttu-id="7af8d-243">Arquivos</span><span class="sxs-lookup"><span data-stu-id="7af8d-243">Files</span></span> |
| [<span data-ttu-id="7af8d-244">/users/{id}/profile</span><span class="sxs-lookup"><span data-stu-id="7af8d-244">/users/{id}/profile</span></span>](/graph/api/profile-get) | <span data-ttu-id="7af8d-245">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7af8d-245">User.Read.All</span></span> | <span data-ttu-id="7af8d-246">Perfil</span><span class="sxs-lookup"><span data-stu-id="7af8d-246">Profile</span></span> |

<span data-ttu-id="7af8d-247">A `MgtPersonCard` classe também expõe um `getScopes` método estático que retorna uma matriz de escopos necessários para que o cartão Person funcione com base na configuração do cartão de pessoa global.</span><span class="sxs-lookup"><span data-stu-id="7af8d-247">The `MgtPersonCard` class also exposes a `getScopes` static method that returns an array of scopes required for the person card to function based on the global person card configuration.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a><span data-ttu-id="7af8d-248">Autenticação</span><span class="sxs-lookup"><span data-stu-id="7af8d-248">Authentication</span></span>

<span data-ttu-id="7af8d-249">O controle Person-Card usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="7af8d-249">The Person-Card control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 
