---
title: Person-Card componente no microsoft graph Toolkit
description: Um Person-Card é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 9c12c9e76f6c0b332a70bfbc429bc7b7845056cb
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266805"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="4b3ab-103">Person-Card componente no microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="4b3ab-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4b3ab-104">Um Person-Card é um componente responsivo para exibir mais informações relacionadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="4b3ab-105">Geralmente, ele é usado como um sobrevoo no `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="4b3ab-106">Para obter mais informações sobre o `mgt-person` componente, consulte [mgt-person](./person.md).</span><span class="sxs-lookup"><span data-stu-id="4b3ab-106">For more information about the `mgt-person` component, see [mgt-person](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="4b3ab-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b3ab-107">Example</span></span>

<span data-ttu-id="4b3ab-108">O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="4b3ab-109">Passe o mouse sobre a pessoa para ver o [](#properties) Cartão de Pessoa e use o editor de código para ver como as propriedades alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="4b3ab-110">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="4b3ab-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a><span data-ttu-id="4b3ab-111">Configuração de componente global</span><span class="sxs-lookup"><span data-stu-id="4b3ab-111">Global component configuration</span></span>

<span data-ttu-id="4b3ab-112">A `MgtPersonCard` classe expõe um objeto `config` estático que configura todos os componentes de cartão de pessoa no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-112">The `MgtPersonCard` class exposes a static `config` object that configures all person card components in the application.</span></span> <span data-ttu-id="4b3ab-113">O objeto config configura quais seções e quais APIs são usadas pelo cartão de pessoa para buscar detalhes sobre um usuário do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-113">The config object configures what sections and what APIs are used by the person card to fetch details about a user from Microsoft Graph.</span></span>

<span data-ttu-id="4b3ab-114">Por padrão, todas as seções e APIs estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-114">By default, all sections and APIs are enabled.</span></span> <span data-ttu-id="4b3ab-115">O exemplo a seguir mostra como usar o objeto config para desabilitar seções ou APIs.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-115">The following example shows how to use the config object to disable sections or APIs.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

<span data-ttu-id="4b3ab-116">As propriedades a seguir estão disponíveis no objeto config.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-116">The following properties are available on the config object.</span></span>

| <span data-ttu-id="4b3ab-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b3ab-117">Property</span></span> | <span data-ttu-id="4b3ab-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3ab-118">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="4b3ab-119">useContactApis</span><span class="sxs-lookup"><span data-stu-id="4b3ab-119">useContactApis</span></span> | <span data-ttu-id="4b3ab-120">`boolean` - Indica se o componente de cartão de pessoa pode usar a API de Contato do Microsoft Graph para pesquisar detalhes de contato e fotos.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-120">`boolean` - Indicates whether the person card component can use the Microsoft Graph Contact API to search for contact details and photos.</span></span> <span data-ttu-id="4b3ab-121">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-121">Default value is `true`.</span></span>  |
| <span data-ttu-id="4b3ab-122">seções</span><span class="sxs-lookup"><span data-stu-id="4b3ab-122">sections</span></span> | <span data-ttu-id="4b3ab-123">`object` - Configura quais seções são mostradas no cartão de pessoa.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-123">`object` - Configures what sections are shown in the person card.</span></span>  |

### <a name="person-card-sections"></a><span data-ttu-id="4b3ab-124">Seções de cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-124">Person card sections</span></span>

<span data-ttu-id="4b3ab-125">O cartão de pessoa contém várias seções configuráveis para exibir detalhes da pessoa:</span><span class="sxs-lookup"><span data-stu-id="4b3ab-125">The person card contains several configurable sections for displaying person details:</span></span>
* <span data-ttu-id="4b3ab-126">Contato - Informações de contato como email, telefone, posição, local e muito mais.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-126">Contact - Contact information such as email, phone, position, location, and more.</span></span>
* <span data-ttu-id="4b3ab-127">Organização - Gráfico organizacional com gerentes, relatórios diretos e pessoas relevantes.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-127">Organization - Organizational graph with managers, direct reports, and relevant people.</span></span>
* <span data-ttu-id="4b3ab-128">Mensagens - Mensagens de email mais relevantes com o usuário atualmente assinado.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-128">Messages - Most relevant email messages with the current signed in user.</span></span>
* <span data-ttu-id="4b3ab-129">Arquivos - Arquivos compartilhados mais relevantes com o usuário atualmente assinado.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-129">Files - Most relevant shared files with the current signed in user.</span></span>
* <span data-ttu-id="4b3ab-130">Perfil - Informações de perfil, como projetos, habilidades, idiomas e muito mais.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-130">Profile - Profile information such as projects, skills, languages, and more.</span></span>

<span data-ttu-id="4b3ab-131">As seções são carregadas por padrão, mas podem ser desabilitadas globalmente por meio `MgtPersonCard.config.sections` da propriedade object.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-131">Sections are loaded by default, but they can be disabled globally via the `MgtPersonCard.config.sections` object property.</span></span> <span data-ttu-id="4b3ab-132">As propriedades a seguir estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-132">The following properties are available.</span></span>

| <span data-ttu-id="4b3ab-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b3ab-133">Property</span></span> | <span data-ttu-id="4b3ab-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3ab-134">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="4b3ab-135">organization</span><span class="sxs-lookup"><span data-stu-id="4b3ab-135">organization</span></span> | <span data-ttu-id="4b3ab-136">`boolean` - Indica se a seção organização do cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-136">`boolean` - Indicates whether the person card organization section is shown.</span></span> <span data-ttu-id="4b3ab-137">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-137">Default value is `true`.</span></span>  |
| <span data-ttu-id="4b3ab-138">mailMessages</span><span class="sxs-lookup"><span data-stu-id="4b3ab-138">mailMessages</span></span> | <span data-ttu-id="4b3ab-139">`boolean` - Indica se a seção mensagens de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-139">`boolean` - Indicates whether the person card messages section is shown.</span></span> <span data-ttu-id="4b3ab-140">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-140">Default value is `true`.</span></span>  |
| <span data-ttu-id="4b3ab-141">arquivos</span><span class="sxs-lookup"><span data-stu-id="4b3ab-141">files</span></span> | <span data-ttu-id="4b3ab-142">`boolean` - Indica se a seção arquivos de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-142">`boolean` - Indicates whether the person card files section is shown.</span></span> <span data-ttu-id="4b3ab-143">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-143">Default value is `true`.</span></span>  |
| <span data-ttu-id="4b3ab-144">perfil</span><span class="sxs-lookup"><span data-stu-id="4b3ab-144">profile</span></span> | <span data-ttu-id="4b3ab-145">`boolean` - Indica se a seção perfil de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-145">`boolean` - Indicates whether the person card profile section is shown.</span></span> <span data-ttu-id="4b3ab-146">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-146">Default value is `true`.</span></span>  |

<span data-ttu-id="4b3ab-147">Para desabilitar uma seção, basta definir a propriedade como `false` no código de inicialização do aplicativo:</span><span class="sxs-lookup"><span data-stu-id="4b3ab-147">To disable a section, simply set the property to `false` in your app initialization code:</span></span>
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="4b3ab-148">Configuração para integrações do Teams</span><span class="sxs-lookup"><span data-stu-id="4b3ab-148">Setup for Teams integrations</span></span>

<span data-ttu-id="4b3ab-149">O Person-Card componente permite que o usuário entre em contato com a pessoa de destino, incluindo por meio do chat do Teams.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-149">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="4b3ab-150">Se usar o componente dentro de um aplicativo de guia do Teams, você pode garantir que o componente se vincula diretamente a um chat em vez de abrir uma janela do navegador definindo `microsoftTeamsLib` o em `TeamsProvider` .</span><span class="sxs-lookup"><span data-stu-id="4b3ab-150">If using the component inside a Teams tab app, you can ensure that the component deep links directly to a chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="4b3ab-151">Se o Person-Card não conseguir detectar a versão livre do Teams, o componente tentará abrir o cliente Web do Teams.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-151">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

<span data-ttu-id="4b3ab-152">Para obter mais informações sobre o `TeamsProvider` provedor, consulte [Provedor do Microsoft Teams](../providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="4b3ab-152">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b3ab-153">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b3ab-153">Properties</span></span>

<span data-ttu-id="4b3ab-154">Por padrão, `mgt-person` o componente passará os detalhes da pessoa para o `mgt-person-card` componente.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-154">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="4b3ab-155">No entanto, você pode usar esses atributos para alterar isso ao tentar emplacar o componente ou ao usar o componente `mgt-person` `mgt-person-card` como um componente autônomo.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-155">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="4b3ab-156">Atributo</span><span class="sxs-lookup"><span data-stu-id="4b3ab-156">Attribute</span></span>         | <span data-ttu-id="4b3ab-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b3ab-157">Type</span></span>                     | <span data-ttu-id="4b3ab-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3ab-158">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="4b3ab-159">person-details</span><span class="sxs-lookup"><span data-stu-id="4b3ab-159">person-details</span></span> | <span data-ttu-id="4b3ab-160">MicrosoftGraph.User</span><span class="sxs-lookup"><span data-stu-id="4b3ab-160">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="4b3ab-161">MicrosoftGraph.Person</span><span class="sxs-lookup"><span data-stu-id="4b3ab-161">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="4b3ab-162">MicrosoftGraph.Contact</span><span class="sxs-lookup"><span data-stu-id="4b3ab-162">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="4b3ab-163">Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-163">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="4b3ab-164">person-image</span><span class="sxs-lookup"><span data-stu-id="4b3ab-164">person-image</span></span>   | <span data-ttu-id="4b3ab-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3ab-165">string</span></span>                    | <span data-ttu-id="4b3ab-166">Uri de imagem relacionado à pessoa exibida no cartão.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-166">Image uri related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="4b3ab-167">inherit-details</span><span class="sxs-lookup"><span data-stu-id="4b3ab-167">inherit-details</span></span>   | <span data-ttu-id="4b3ab-168">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-168">None.</span></span>                  | <span data-ttu-id="4b3ab-169">Permite que o cartão de pessoa ande na árvore pai para `mgt-person` que o componente use os mesmos e os `person-details` `person-image` dados.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-169">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="4b3ab-170">user-id</span><span class="sxs-lookup"><span data-stu-id="4b3ab-170">user-id</span></span> | <span data-ttu-id="4b3ab-171">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3ab-171">string</span></span> | <span data-ttu-id="4b3ab-172">Permite que os desenvolvedores fornecem a ID do usuário para recuperar dados mostrados no componente person-card</span><span class="sxs-lookup"><span data-stu-id="4b3ab-172">Allows developers to supply user-id to retrieve data shown on person-card component</span></span> |
| <span data-ttu-id="4b3ab-173">person-query</span><span class="sxs-lookup"><span data-stu-id="4b3ab-173">person-query</span></span> | <span data-ttu-id="4b3ab-174">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b3ab-174">string</span></span> | <span data-ttu-id="4b3ab-175">Permite que os desenvolvedores fornecem consulta de pessoa para recuperar dados mostrados no componente person-card</span><span class="sxs-lookup"><span data-stu-id="4b3ab-175">Allows developers to supply person-query to retrieve data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="4b3ab-176">Modelos</span><span class="sxs-lookup"><span data-stu-id="4b3ab-176">Templates</span></span>

<span data-ttu-id="4b3ab-177">O Person-Card componente usa [modelos](../customize-components/templates.md) que permitem adicionar ou substituir partes do componente.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-177">The Person-Card component uses [templates](../customize-components/templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="4b3ab-178">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-178">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="4b3ab-179">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="4b3ab-179">Data type</span></span> | <span data-ttu-id="4b3ab-180">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="4b3ab-180">Data context</span></span> | <span data-ttu-id="4b3ab-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3ab-181">Description</span></span> |
| - | - | - |
| <span data-ttu-id="4b3ab-182">no-data</span><span class="sxs-lookup"><span data-stu-id="4b3ab-182">no-data</span></span> | <span data-ttu-id="4b3ab-183">null</span><span class="sxs-lookup"><span data-stu-id="4b3ab-183">null</span></span> | <span data-ttu-id="4b3ab-184">O modelo usado quando nenhum dado está disponível.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-184">The template used when no data is available.</span></span>
| <span data-ttu-id="4b3ab-185">Padrão.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-185">default</span></span> | <span data-ttu-id="4b3ab-186">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-186">`person`: The person details object</span></span> <br> <span data-ttu-id="4b3ab-187">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="4b3ab-187">`personImage`: The URL of the image</span></span> | <span data-ttu-id="4b3ab-188">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-188">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="4b3ab-189">person-details</span><span class="sxs-lookup"><span data-stu-id="4b3ab-189">person-details</span></span> | <span data-ttu-id="4b3ab-190">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-190">`person`: The person details object</span></span> | <span data-ttu-id="4b3ab-191">O modelo usado para renderizar a parte superior do cartão de pessoa.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-191">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="4b3ab-192">detalhes adicionais</span><span class="sxs-lookup"><span data-stu-id="4b3ab-192">additional-details</span></span> | <span data-ttu-id="4b3ab-193">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-193">`person`: The person details object</span></span> <br> <span data-ttu-id="4b3ab-194">`personImage`: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="4b3ab-194">`personImage`: the URL of the image</span></span> | <span data-ttu-id="4b3ab-195">O modelo usado para adicionar conteúdo personalizado ao contêiner de detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-195">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="4b3ab-196">Por exemplo, você pode usar um modelo para personalizar o componente anexado ao componente e um modelo para adicionar `mgt-person` detalhes adicionais no cartão.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-196">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="css-custom-properties"></a><span data-ttu-id="4b3ab-197">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="4b3ab-197">CSS custom properties</span></span>

<span data-ttu-id="4b3ab-198">O `mgt-person-card` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-198">The `mgt-person-card` component defines the following CSS custom properties.</span></span> 

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

<span data-ttu-id="4b3ab-199">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="4b3ab-199">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="4b3ab-200">APIs e permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4b3ab-200">Microsoft Graph APIs and permissions</span></span>

<span data-ttu-id="4b3ab-201">O Person-Card usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-201">The Person-Card control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="4b3ab-202">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b3ab-202">Resource</span></span> | <span data-ttu-id="4b3ab-203">Permissão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-203">Permission</span></span> | <span data-ttu-id="4b3ab-204">Section</span><span class="sxs-lookup"><span data-stu-id="4b3ab-204">Section</span></span> |
| - | - | - |
| [<span data-ttu-id="4b3ab-205">/me</span><span class="sxs-lookup"><span data-stu-id="4b3ab-205">/me</span></span>](/graph/api/user-get) | <span data-ttu-id="4b3ab-206">User.Read</span><span class="sxs-lookup"><span data-stu-id="4b3ab-206">User.Read</span></span> | <span data-ttu-id="4b3ab-207">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-207">Default</span></span> |
| [<span data-ttu-id="4b3ab-208">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="4b3ab-208">/me/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="4b3ab-209">User.Read</span><span class="sxs-lookup"><span data-stu-id="4b3ab-209">User.Read</span></span> | <span data-ttu-id="4b3ab-210">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-210">Default</span></span> |
| [<span data-ttu-id="4b3ab-211">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="4b3ab-211">/me/people/?$search=</span></span>](/graph/api/user-list-people) | <span data-ttu-id="4b3ab-212">People.Read</span><span class="sxs-lookup"><span data-stu-id="4b3ab-212">People.Read</span></span> | <span data-ttu-id="4b3ab-213">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-213">Default</span></span> |
| [<span data-ttu-id="4b3ab-214">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="4b3ab-214">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="4b3ab-215">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4b3ab-215">Contacts.Read</span></span> | <span data-ttu-id="4b3ab-216">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-216">Default</span></span> |
| [<span data-ttu-id="4b3ab-217">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="4b3ab-217">/users/{id}</span></span>](/graph/api/user-list-people) | <span data-ttu-id="4b3ab-218">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-218">User.ReadBasic.All</span></span> | <span data-ttu-id="4b3ab-219">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-219">Default</span></span> |
| [<span data-ttu-id="4b3ab-220">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="4b3ab-220">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="4b3ab-221">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-221">User.ReadBasic.All</span></span> | <span data-ttu-id="4b3ab-222">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-222">Default</span></span> |
| [<span data-ttu-id="4b3ab-223">/me/presence</span><span class="sxs-lookup"><span data-stu-id="4b3ab-223">/me/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="4b3ab-224">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="4b3ab-224">Presence.Read</span></span> | <span data-ttu-id="4b3ab-225">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-225">Default</span></span> |
| [<span data-ttu-id="4b3ab-226">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="4b3ab-226">/users/{id}/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="4b3ab-227">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-227">Presence.Read.All</span></span> | <span data-ttu-id="4b3ab-228">Padrão</span><span class="sxs-lookup"><span data-stu-id="4b3ab-228">Default</span></span> |
| [<span data-ttu-id="4b3ab-229">/users/{id}/manager</span><span class="sxs-lookup"><span data-stu-id="4b3ab-229">/users/{id}/manager</span></span>](/graph/api/user-list-manager) | <span data-ttu-id="4b3ab-230">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-230">User.Read.All</span></span> | <span data-ttu-id="4b3ab-231">Organização</span><span class="sxs-lookup"><span data-stu-id="4b3ab-231">Organization</span></span> |
| [<span data-ttu-id="4b3ab-232">/users/{id}/directReports</span><span class="sxs-lookup"><span data-stu-id="4b3ab-232">/users/{id}/directReports</span></span>](/graph/api/user-list-directreports) | <span data-ttu-id="4b3ab-233">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-233">User.Read.All</span></span> | <span data-ttu-id="4b3ab-234">Organização</span><span class="sxs-lookup"><span data-stu-id="4b3ab-234">Organization</span></span> |
| [<span data-ttu-id="4b3ab-235">/users/{id}/people</span><span class="sxs-lookup"><span data-stu-id="4b3ab-235">/users/{id}/people</span></span>](/graph/api/user-list-people) | <span data-ttu-id="4b3ab-236">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-236">People.Read.All</span></span> | <span data-ttu-id="4b3ab-237">Organização</span><span class="sxs-lookup"><span data-stu-id="4b3ab-237">Organization</span></span> |
| [<span data-ttu-id="4b3ab-238">/me/messages</span><span class="sxs-lookup"><span data-stu-id="4b3ab-238">/me/messages</span></span>](/graph/api/user-list-messages) | <span data-ttu-id="4b3ab-239">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="4b3ab-239">Mail.ReadBasic</span></span> | <span data-ttu-id="4b3ab-240">Mensagens</span><span class="sxs-lookup"><span data-stu-id="4b3ab-240">Messages</span></span> |
| <span data-ttu-id="4b3ab-241">[/me/insights/shared](/graph/api/insights-list-shared) e [/me/insights/used](/graph/api/insights-list-used)</span><span class="sxs-lookup"><span data-stu-id="4b3ab-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span></span> | <span data-ttu-id="4b3ab-242">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-242">Sites.Read.All</span></span> | <span data-ttu-id="4b3ab-243">Arquivos</span><span class="sxs-lookup"><span data-stu-id="4b3ab-243">Files</span></span> |
| [<span data-ttu-id="4b3ab-244">/users/{id}/profile</span><span class="sxs-lookup"><span data-stu-id="4b3ab-244">/users/{id}/profile</span></span>](/graph/api/profile-get) | <span data-ttu-id="4b3ab-245">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3ab-245">User.Read.All</span></span> | <span data-ttu-id="4b3ab-246">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b3ab-246">Profile</span></span> |

<span data-ttu-id="4b3ab-247">A classe também expõe um método estático que retorna uma matriz de escopos necessários para que o cartão de pessoa funcione com base na configuração `MgtPersonCard` global do cartão de `getScopes` pessoa.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-247">The `MgtPersonCard` class also exposes a `getScopes` static method that returns an array of scopes required for the person card to function based on the global person card configuration.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a><span data-ttu-id="4b3ab-248">Autenticação</span><span class="sxs-lookup"><span data-stu-id="4b3ab-248">Authentication</span></span>

<span data-ttu-id="4b3ab-249">O Person-Card usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="4b3ab-249">The Person-Card control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="4b3ab-250">Cache</span><span class="sxs-lookup"><span data-stu-id="4b3ab-250">Cache</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4b3ab-251">O `mgt-person-card` componente recupera os dados básicos da pessoa do componente pai sem chamar o Microsoft `mgt-person` Graph.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-251">The `mgt-person-card` component retrieves the basic person data from the parent `mgt-person` component without calling Microsoft Graph.</span></span> <span data-ttu-id="4b3ab-252">Quando `mgt-person-card` for usado separadamente, ele recuperará os dados necessários em si e os armazenará em cache.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-252">When `mgt-person-card` is used separately, it will retrieve the necessary data itself and cache it.</span></span> <span data-ttu-id="4b3ab-253">Os dados exibidos nas seções do cartão são recuperados separadamente e não são armazenados em cache.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-253">The data displayed in card's sections is retrieved separately and is not cached.</span></span>

|<span data-ttu-id="4b3ab-254">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="4b3ab-254">Object store</span></span>|<span data-ttu-id="4b3ab-255">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="4b3ab-255">Cached data</span></span>|<span data-ttu-id="4b3ab-256">Comentários</span><span class="sxs-lookup"><span data-stu-id="4b3ab-256">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="4b3ab-257">Informações da pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-257">Person's information</span></span>|<span data-ttu-id="4b3ab-258">Usado quando `personQuery` especificado e seu valor é diferente do `me`</span><span class="sxs-lookup"><span data-stu-id="4b3ab-258">Used when `personQuery` is specified and its value is different than `me`</span></span>|
|`photos`|<span data-ttu-id="4b3ab-259">Foto da pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-259">Person's photo</span></span>|
|`presence`|<span data-ttu-id="4b3ab-260">Presença da pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-260">Person's presence</span></span>|<span data-ttu-id="4b3ab-261">Usado, quando `showPresence` está definido como `true`</span><span class="sxs-lookup"><span data-stu-id="4b3ab-261">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="4b3ab-262">Informações do usuário da pessoa</span><span class="sxs-lookup"><span data-stu-id="4b3ab-262">Person's user information</span></span>|<span data-ttu-id="4b3ab-263">Usado quando `userId` especificado ou `personQuery` definido como `me`</span><span class="sxs-lookup"><span data-stu-id="4b3ab-263">Used when `userId` is specified or the `personQuery` is set to `me`</span></span>|

<span data-ttu-id="4b3ab-264">Consulte [Cache para](../customize-components/cache.md) obter mais detalhes sobre como configurar o cache.</span><span class="sxs-lookup"><span data-stu-id="4b3ab-264">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
