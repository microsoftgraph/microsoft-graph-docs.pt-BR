---
title: Person-Card componente no microsoft Graph Toolkit
description: Um Person-Card é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 23f26927935af3f3123e4f812853475cb8a0a9dc
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082038"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="bb051-103">Person-Card componente no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bb051-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bb051-104">Um Person-Card é um componente responsivo para exibir mais informações relacionadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="bb051-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="bb051-105">Geralmente, ele é usado como um sobrevoo no `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="bb051-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="bb051-106">Para obter mais informações sobre o `mgt-person` componente, consulte [mgt-person](./person.md).</span><span class="sxs-lookup"><span data-stu-id="bb051-106">For more information about the `mgt-person` component, see [mgt-person](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="bb051-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb051-107">Example</span></span>

<span data-ttu-id="bb051-108">O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="bb051-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="bb051-109">Passe o mouse sobre a pessoa para ver o [](#properties) Cartão de Pessoa e use o editor de código para ver como as propriedades alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="bb051-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[<span data-ttu-id="bb051-110">Abrir este exemplo no mgt.dev</span><span class="sxs-lookup"><span data-stu-id="bb051-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a><span data-ttu-id="bb051-111">Configuração de componente global</span><span class="sxs-lookup"><span data-stu-id="bb051-111">Global component configuration</span></span>

<span data-ttu-id="bb051-112">A `MgtPersonCard` classe expõe um objeto `config` estático que configura todos os componentes de cartão de pessoa no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bb051-112">The `MgtPersonCard` class exposes a static `config` object that configures all person card components in the application.</span></span> <span data-ttu-id="bb051-113">O objeto config configura quais seções e quais APIs são usadas pelo cartão de pessoa para buscar detalhes sobre um usuário do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bb051-113">The config object configures what sections and what APIs are used by the person card to fetch details about a user from Microsoft Graph.</span></span>

<span data-ttu-id="bb051-114">Por padrão, todas as seções e APIs estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="bb051-114">By default, all sections and APIs are enabled.</span></span> <span data-ttu-id="bb051-115">O exemplo a seguir mostra como usar o objeto config para desabilitar seções ou APIs.</span><span class="sxs-lookup"><span data-stu-id="bb051-115">The following example shows how to use the config object to disable sections or APIs.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

<span data-ttu-id="bb051-116">As propriedades a seguir estão disponíveis no objeto config.</span><span class="sxs-lookup"><span data-stu-id="bb051-116">The following properties are available on the config object.</span></span>

| <span data-ttu-id="bb051-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb051-117">Property</span></span> | <span data-ttu-id="bb051-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb051-118">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="bb051-119">useContactApis</span><span class="sxs-lookup"><span data-stu-id="bb051-119">useContactApis</span></span> | <span data-ttu-id="bb051-120">`boolean`- Indica se o componente de cartão de pessoa pode usar a API de contato do Microsoft Graph para pesquisar detalhes e fotos de contato.</span><span class="sxs-lookup"><span data-stu-id="bb051-120">`boolean` - Indicates whether the person card component can use the Microsoft Graph Contact API to search for contact details and photos.</span></span> <span data-ttu-id="bb051-121">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="bb051-121">Default value is `true`.</span></span>  |
| <span data-ttu-id="bb051-122">seções</span><span class="sxs-lookup"><span data-stu-id="bb051-122">sections</span></span> | <span data-ttu-id="bb051-123">`object` - Configura quais seções são mostradas no cartão de pessoa.</span><span class="sxs-lookup"><span data-stu-id="bb051-123">`object` - Configures what sections are shown in the person card.</span></span>  |

### <a name="person-card-sections"></a><span data-ttu-id="bb051-124">Seções de cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-124">Person card sections</span></span>

<span data-ttu-id="bb051-125">O cartão de pessoa contém várias seções configuráveis para exibir detalhes da pessoa:</span><span class="sxs-lookup"><span data-stu-id="bb051-125">The person card contains several configurable sections for displaying person details:</span></span>
* <span data-ttu-id="bb051-126">Contato - Informações de contato como email, telefone, posição, local e muito mais.</span><span class="sxs-lookup"><span data-stu-id="bb051-126">Contact - Contact information such as email, phone, position, location, and more.</span></span>
* <span data-ttu-id="bb051-127">Organização - Gráfico organizacional com gerentes, relatórios diretos e pessoas relevantes.</span><span class="sxs-lookup"><span data-stu-id="bb051-127">Organization - Organizational graph with managers, direct reports, and relevant people.</span></span>
* <span data-ttu-id="bb051-128">Mensagens - Mensagens de email mais relevantes com o usuário atualmente assinado.</span><span class="sxs-lookup"><span data-stu-id="bb051-128">Messages - Most relevant email messages with the current signed in user.</span></span>
* <span data-ttu-id="bb051-129">Arquivos - Arquivos compartilhados mais relevantes com o usuário atualmente assinado.</span><span class="sxs-lookup"><span data-stu-id="bb051-129">Files - Most relevant shared files with the current signed in user.</span></span>
* <span data-ttu-id="bb051-130">Perfil - Informações de perfil, como projetos, habilidades, idiomas e muito mais.</span><span class="sxs-lookup"><span data-stu-id="bb051-130">Profile - Profile information such as projects, skills, languages, and more.</span></span>

<span data-ttu-id="bb051-131">As seções são carregadas por padrão, mas podem ser desabilitadas globalmente por meio `MgtPersonCard.config.sections` da propriedade object.</span><span class="sxs-lookup"><span data-stu-id="bb051-131">Sections are loaded by default, but they can be disabled globally via the `MgtPersonCard.config.sections` object property.</span></span> <span data-ttu-id="bb051-132">As propriedades a seguir estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="bb051-132">The following properties are available.</span></span>

| <span data-ttu-id="bb051-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb051-133">Property</span></span> | <span data-ttu-id="bb051-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb051-134">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="bb051-135">organization</span><span class="sxs-lookup"><span data-stu-id="bb051-135">organization</span></span> | <span data-ttu-id="bb051-136">`boolean` - Indica se a seção organização do cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="bb051-136">`boolean` - Indicates whether the person card organization section is shown.</span></span> <span data-ttu-id="bb051-137">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="bb051-137">Default value is `true`.</span></span>  |
| <span data-ttu-id="bb051-138">mailMessages</span><span class="sxs-lookup"><span data-stu-id="bb051-138">mailMessages</span></span> | <span data-ttu-id="bb051-139">`boolean` - Indica se a seção mensagens de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="bb051-139">`boolean` - Indicates whether the person card messages section is shown.</span></span> <span data-ttu-id="bb051-140">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="bb051-140">Default value is `true`.</span></span>  |
| <span data-ttu-id="bb051-141">arquivos</span><span class="sxs-lookup"><span data-stu-id="bb051-141">files</span></span> | <span data-ttu-id="bb051-142">`boolean` - Indica se a seção arquivos de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="bb051-142">`boolean` - Indicates whether the person card files section is shown.</span></span> <span data-ttu-id="bb051-143">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="bb051-143">Default value is `true`.</span></span>  |
| <span data-ttu-id="bb051-144">perfil</span><span class="sxs-lookup"><span data-stu-id="bb051-144">profile</span></span> | <span data-ttu-id="bb051-145">`boolean` - Indica se a seção perfil de cartão de pessoa é mostrada.</span><span class="sxs-lookup"><span data-stu-id="bb051-145">`boolean` - Indicates whether the person card profile section is shown.</span></span> <span data-ttu-id="bb051-146">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="bb051-146">Default value is `true`.</span></span>  |

<span data-ttu-id="bb051-147">Para desabilitar uma seção, basta definir a propriedade como `false` no código de inicialização do aplicativo:</span><span class="sxs-lookup"><span data-stu-id="bb051-147">To disable a section, simply set the property to `false` in your app initialization code:</span></span>
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="bb051-148">Instalação para Teams integrações</span><span class="sxs-lookup"><span data-stu-id="bb051-148">Setup for Teams integrations</span></span>

<span data-ttu-id="bb051-149">O Person-Card componente permite que o usuário entre em contato com a pessoa de destino, incluindo Teams chat.</span><span class="sxs-lookup"><span data-stu-id="bb051-149">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="bb051-150">Se usar o componente dentro de um aplicativo de guia Teams, você pode garantir que o componente se vincula diretamente a um chat em vez de abrir uma janela do navegador definindo o `microsoftTeamsLib` em `TeamsProvider` .</span><span class="sxs-lookup"><span data-stu-id="bb051-150">If using the component inside a Teams tab app, you can ensure that the component deep links directly to a chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="bb051-151">Se o Person-Card não puder detectar a Teams, o componente tentará abrir o cliente Teams Web.</span><span class="sxs-lookup"><span data-stu-id="bb051-151">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

<span data-ttu-id="bb051-152">Para obter mais informações sobre o `TeamsProvider` provedor, [consulte Microsoft Teams provedor](../providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="bb051-152">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bb051-153">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb051-153">Properties</span></span>

<span data-ttu-id="bb051-154">Por padrão, `mgt-person` o componente passará os detalhes da pessoa para o `mgt-person-card` componente.</span><span class="sxs-lookup"><span data-stu-id="bb051-154">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="bb051-155">No entanto, você pode usar esses atributos para alterar isso ao tentar emplacar o componente ou ao usar o componente `mgt-person` `mgt-person-card` como um componente autônomo.</span><span class="sxs-lookup"><span data-stu-id="bb051-155">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="bb051-156">Atributo</span><span class="sxs-lookup"><span data-stu-id="bb051-156">Attribute</span></span>         | <span data-ttu-id="bb051-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb051-157">Type</span></span>                     | <span data-ttu-id="bb051-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb051-158">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="bb051-159">person-details</span><span class="sxs-lookup"><span data-stu-id="bb051-159">person-details</span></span> | <span data-ttu-id="bb051-160">MicrosoftGraph.User</span><span class="sxs-lookup"><span data-stu-id="bb051-160">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="bb051-161">MicrosoftGraph.Person</span><span class="sxs-lookup"><span data-stu-id="bb051-161">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="bb051-162">MicrosoftGraph.Contact</span><span class="sxs-lookup"><span data-stu-id="bb051-162">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="bb051-163">Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="bb051-163">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="bb051-164">person-image</span><span class="sxs-lookup"><span data-stu-id="bb051-164">person-image</span></span>   | <span data-ttu-id="bb051-165">string</span><span class="sxs-lookup"><span data-stu-id="bb051-165">string</span></span>                    | <span data-ttu-id="bb051-166">Uri de imagem relacionado à pessoa exibida no cartão.</span><span class="sxs-lookup"><span data-stu-id="bb051-166">Image uri related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="bb051-167">inherit-details</span><span class="sxs-lookup"><span data-stu-id="bb051-167">inherit-details</span></span>   | <span data-ttu-id="bb051-168">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bb051-168">None.</span></span>                  | <span data-ttu-id="bb051-169">Permite que o cartão de pessoa ande na árvore pai para `mgt-person` que o componente use os mesmos e os `person-details` `person-image` dados.</span><span class="sxs-lookup"><span data-stu-id="bb051-169">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="bb051-170">user-id</span><span class="sxs-lookup"><span data-stu-id="bb051-170">user-id</span></span> | <span data-ttu-id="bb051-171">string</span><span class="sxs-lookup"><span data-stu-id="bb051-171">string</span></span> | <span data-ttu-id="bb051-172">Permite que os desenvolvedores fornecem a ID do usuário para recuperar dados mostrados no componente person-card</span><span class="sxs-lookup"><span data-stu-id="bb051-172">Allows developers to supply user-id to retrieve data shown on person-card component</span></span> |
| <span data-ttu-id="bb051-173">person-query</span><span class="sxs-lookup"><span data-stu-id="bb051-173">person-query</span></span> | <span data-ttu-id="bb051-174">string</span><span class="sxs-lookup"><span data-stu-id="bb051-174">string</span></span> | <span data-ttu-id="bb051-175">Permite que os desenvolvedores fornecem consulta de pessoa para recuperar dados mostrados no componente person-card</span><span class="sxs-lookup"><span data-stu-id="bb051-175">Allows developers to supply person-query to retrieve data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="bb051-176">Modelos</span><span class="sxs-lookup"><span data-stu-id="bb051-176">Templates</span></span>

<span data-ttu-id="bb051-177">O Person-Card componente usa [modelos](../customize-components/templates.md) que permitem adicionar ou substituir partes do componente.</span><span class="sxs-lookup"><span data-stu-id="bb051-177">The Person-Card component uses [templates](../customize-components/templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="bb051-178">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="bb051-178">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="bb051-179">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="bb051-179">Data type</span></span> | <span data-ttu-id="bb051-180">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="bb051-180">Data context</span></span> | <span data-ttu-id="bb051-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb051-181">Description</span></span> |
| - | - | - |
| <span data-ttu-id="bb051-182">no-data</span><span class="sxs-lookup"><span data-stu-id="bb051-182">no-data</span></span> | <span data-ttu-id="bb051-183">null</span><span class="sxs-lookup"><span data-stu-id="bb051-183">null</span></span> | <span data-ttu-id="bb051-184">O modelo usado quando nenhum dado está disponível.</span><span class="sxs-lookup"><span data-stu-id="bb051-184">The template used when no data is available.</span></span>
| <span data-ttu-id="bb051-185">Padrão.</span><span class="sxs-lookup"><span data-stu-id="bb051-185">default</span></span> | <span data-ttu-id="bb051-186">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-186">`person`: The person details object</span></span> <br> <span data-ttu-id="bb051-187">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="bb051-187">`personImage`: The URL of the image</span></span> | <span data-ttu-id="bb051-188">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="bb051-188">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="bb051-189">person-details</span><span class="sxs-lookup"><span data-stu-id="bb051-189">person-details</span></span> | <span data-ttu-id="bb051-190">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-190">`person`: The person details object</span></span> | <span data-ttu-id="bb051-191">O modelo usado para renderizar a parte superior do cartão de pessoa.</span><span class="sxs-lookup"><span data-stu-id="bb051-191">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="bb051-192">detalhes adicionais</span><span class="sxs-lookup"><span data-stu-id="bb051-192">additional-details</span></span> | <span data-ttu-id="bb051-193">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-193">`person`: The person details object</span></span> <br> <span data-ttu-id="bb051-194">`personImage`: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="bb051-194">`personImage`: the URL of the image</span></span> | <span data-ttu-id="bb051-195">O modelo usado para adicionar conteúdo personalizado ao contêiner de detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="bb051-195">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="bb051-196">Por exemplo, você pode usar um modelo para personalizar o componente anexado ao componente e um modelo para adicionar `mgt-person` detalhes adicionais no cartão.</span><span class="sxs-lookup"><span data-stu-id="bb051-196">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="events"></a><span data-ttu-id="bb051-197">Eventos</span><span class="sxs-lookup"><span data-stu-id="bb051-197">Events</span></span>

<span data-ttu-id="bb051-198">Os eventos a seguir são disparados do componente.</span><span class="sxs-lookup"><span data-stu-id="bb051-198">The following events are fired from the component.</span></span>

| <span data-ttu-id="bb051-199">Evento</span><span class="sxs-lookup"><span data-stu-id="bb051-199">Event</span></span> | <span data-ttu-id="bb051-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb051-200">Description</span></span> |
| --- | --- |
| `expanded` | <span data-ttu-id="bb051-201">O usuário abriu a seção detalhes expandidos do cartão.</span><span class="sxs-lookup"><span data-stu-id="bb051-201">The user has opened the expanded details section of the card.</span></span> |

<span data-ttu-id="bb051-202">Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).</span><span class="sxs-lookup"><span data-stu-id="bb051-202">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="css-custom-properties"></a><span data-ttu-id="bb051-203">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="bb051-203">CSS custom properties</span></span>

<span data-ttu-id="bb051-204">O `mgt-person-card` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="bb051-204">The `mgt-person-card` component defines the following CSS custom properties.</span></span> 

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

<span data-ttu-id="bb051-205">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="bb051-205">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="bb051-206">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bb051-206">Microsoft Graph permissions</span></span>

<span data-ttu-id="bb051-207">O controle Person-Card usa as seguintes APIs Graph Microsoft e permissões.</span><span class="sxs-lookup"><span data-stu-id="bb051-207">The Person-Card control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="bb051-208">Configuração</span><span class="sxs-lookup"><span data-stu-id="bb051-208">Configuration</span></span> | <span data-ttu-id="bb051-209">Permissão</span><span class="sxs-lookup"><span data-stu-id="bb051-209">Permission</span></span> | <span data-ttu-id="bb051-210">API</span><span class="sxs-lookup"><span data-stu-id="bb051-210">API</span></span> | <span data-ttu-id="bb051-211">Section</span><span class="sxs-lookup"><span data-stu-id="bb051-211">Section</span></span> |
| --- | ---------- | ------- | --------- |
| <span data-ttu-id="bb051-212">`personDetails` set with user's `id` but without e-mail, or `userId` set, or set `personQuery` to `me`</span><span class="sxs-lookup"><span data-stu-id="bb051-212">`personDetails` set with user's `id` but without e-mail, or `userId` set, or `personQuery` set to `me`</span></span> | <span data-ttu-id="bb051-213">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="bb051-213">User.ReadBasic.All</span></span> | <span data-ttu-id="bb051-214">[/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get)</span><span class="sxs-lookup"><span data-stu-id="bb051-214">[/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get)</span></span> | <span data-ttu-id="bb051-215">Padrão</span><span class="sxs-lookup"><span data-stu-id="bb051-215">Default</span></span> |
| <span data-ttu-id="bb051-216">`personQuery` definido como um valor diferente do `me`</span><span class="sxs-lookup"><span data-stu-id="bb051-216">`personQuery` set to a value different than `me`</span></span> | <span data-ttu-id="bb051-217">People.Read</span><span class="sxs-lookup"><span data-stu-id="bb051-217">People.Read</span></span> | [<span data-ttu-id="bb051-218">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="bb051-218">/me/people/?$search=</span></span>](/graph/api/user-list-people) | <span data-ttu-id="bb051-219">Padrão</span><span class="sxs-lookup"><span data-stu-id="bb051-219">Default</span></span> |
| <span data-ttu-id="bb051-220">`personQuery` definido como um valor diferente `me` e `config.useContactApis` definido como `true` (padrão)</span><span class="sxs-lookup"><span data-stu-id="bb051-220">`personQuery` set to a value different than `me` and `config.useContactApis` set to `true` (default)</span></span> | <span data-ttu-id="bb051-221">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bb051-221">Contacts.Read</span></span> | [<span data-ttu-id="bb051-222">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="bb051-222">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="bb051-223">Padrão</span><span class="sxs-lookup"><span data-stu-id="bb051-223">Default</span></span> |
| <span data-ttu-id="bb051-224">`showPresence` set to `true`</span><span class="sxs-lookup"><span data-stu-id="bb051-224">`showPresence` set to `true`</span></span> | <span data-ttu-id="bb051-225">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb051-225">Presence.Read.All</span></span> | [<span data-ttu-id="bb051-226">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="bb051-226">/users/{id}/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="bb051-227">Padrão</span><span class="sxs-lookup"><span data-stu-id="bb051-227">Default</span></span> |
| <span data-ttu-id="bb051-228">`sections.organization` habilitado (padrão)</span><span class="sxs-lookup"><span data-stu-id="bb051-228">`sections.organization` enabled (default)</span></span> | <span data-ttu-id="bb051-229">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb051-229">User.Read.All</span></span> | [<span data-ttu-id="bb051-230">/users/{id}/manager</span><span class="sxs-lookup"><span data-stu-id="bb051-230">/users/{id}/manager</span></span>](/graph/api/user-list-manager) | <span data-ttu-id="bb051-231">Organização</span><span class="sxs-lookup"><span data-stu-id="bb051-231">Organization</span></span> |
| <span data-ttu-id="bb051-232">`sections.organization.showWorksWith` set (padrão)</span><span class="sxs-lookup"><span data-stu-id="bb051-232">`sections.organization.showWorksWith` set (default)</span></span> | <span data-ttu-id="bb051-233">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb051-233">People.Read.All</span></span> | [<span data-ttu-id="bb051-234">/users/{id}/people</span><span class="sxs-lookup"><span data-stu-id="bb051-234">/users/{id}/people</span></span>](/graph/api/user-list-people) | <span data-ttu-id="bb051-235">Organização</span><span class="sxs-lookup"><span data-stu-id="bb051-235">Organization</span></span> |
| <span data-ttu-id="bb051-236">`sections.mailMessages` habilitado (padrão)</span><span class="sxs-lookup"><span data-stu-id="bb051-236">`sections.mailMessages` enabled (default)</span></span> | <span data-ttu-id="bb051-237">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="bb051-237">Mail.ReadBasic</span></span> | [<span data-ttu-id="bb051-238">/me/messages</span><span class="sxs-lookup"><span data-stu-id="bb051-238">/me/messages</span></span>](/graph/api/user-list-messages) | <span data-ttu-id="bb051-239">Mensagens</span><span class="sxs-lookup"><span data-stu-id="bb051-239">Messages</span></span> |
| <span data-ttu-id="bb051-240">`sections.files` habilitado (padrão)</span><span class="sxs-lookup"><span data-stu-id="bb051-240">`sections.files` enabled (default)</span></span> | <span data-ttu-id="bb051-241">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb051-241">Sites.Read.All</span></span> | <span data-ttu-id="bb051-242">[/me/insights/shared](/graph/api/insights-list-shared) e [/me/insights/used](/graph/api/insights-list-used)</span><span class="sxs-lookup"><span data-stu-id="bb051-242">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span></span> | <span data-ttu-id="bb051-243">Arquivos</span><span class="sxs-lookup"><span data-stu-id="bb051-243">Files</span></span> |

<span data-ttu-id="bb051-244">A classe também expõe um método estático que retorna uma matriz de escopos necessários para que o cartão de pessoa funcione com base na configuração `MgtPersonCard` global do cartão de `getScopes` pessoa.</span><span class="sxs-lookup"><span data-stu-id="bb051-244">The `MgtPersonCard` class also exposes a `getScopes` static method that returns an array of scopes required for the person card to function based on the global person card configuration.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a><span data-ttu-id="bb051-245">Autenticação</span><span class="sxs-lookup"><span data-stu-id="bb051-245">Authentication</span></span>

<span data-ttu-id="bb051-246">O Person-Card usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="bb051-246">The Person-Card control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="bb051-247">Cache</span><span class="sxs-lookup"><span data-stu-id="bb051-247">Cache</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bb051-248">O `mgt-person-card` componente recupera os dados básicos da pessoa do componente pai sem chamar o Microsoft `mgt-person` Graph.</span><span class="sxs-lookup"><span data-stu-id="bb051-248">The `mgt-person-card` component retrieves the basic person data from the parent `mgt-person` component without calling Microsoft Graph.</span></span> <span data-ttu-id="bb051-249">Quando `mgt-person-card` for usado separadamente, ele recuperará os dados necessários em si e os armazenará em cache.</span><span class="sxs-lookup"><span data-stu-id="bb051-249">When `mgt-person-card` is used separately, it will retrieve the necessary data itself and cache it.</span></span> <span data-ttu-id="bb051-250">Os dados exibidos nas seções do cartão são recuperados separadamente e não são armazenados em cache.</span><span class="sxs-lookup"><span data-stu-id="bb051-250">The data displayed in card's sections is retrieved separately and is not cached.</span></span>

|<span data-ttu-id="bb051-251">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="bb051-251">Object store</span></span>|<span data-ttu-id="bb051-252">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="bb051-252">Cached data</span></span>|<span data-ttu-id="bb051-253">Comentários</span><span class="sxs-lookup"><span data-stu-id="bb051-253">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="bb051-254">Informações da pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-254">Person's information</span></span>|<span data-ttu-id="bb051-255">Usado quando `personQuery` especificado e seu valor é diferente do `me`</span><span class="sxs-lookup"><span data-stu-id="bb051-255">Used when `personQuery` is specified and its value is different than `me`</span></span>|
|`photos`|<span data-ttu-id="bb051-256">Foto da pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-256">Person's photo</span></span>|
|`presence`|<span data-ttu-id="bb051-257">Presença da pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-257">Person's presence</span></span>|<span data-ttu-id="bb051-258">Usado, quando `showPresence` está definido como `true`</span><span class="sxs-lookup"><span data-stu-id="bb051-258">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="bb051-259">Informações do usuário da pessoa</span><span class="sxs-lookup"><span data-stu-id="bb051-259">Person's user information</span></span>|<span data-ttu-id="bb051-260">Usado quando `userId` especificado ou `personQuery` definido como `me`</span><span class="sxs-lookup"><span data-stu-id="bb051-260">Used when `userId` is specified or the `personQuery` is set to `me`</span></span>|

<span data-ttu-id="bb051-261">Consulte [Caching](../customize-components/cache.md) para obter mais detalhes sobre como configurar o cache.</span><span class="sxs-lookup"><span data-stu-id="bb051-261">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
