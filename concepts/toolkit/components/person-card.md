---
title: Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph
description: Um componente de cartão de pessoa é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 3d440f1340f9ee3f40c37538b1befcacd9867dc1
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144286"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9b06d-103">Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b06d-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9b06d-104">Um componente de cartão de pessoa é um componente responsivo para exibir mais informações relacionadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="9b06d-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="9b06d-105">Geralmente, é usado como um submenu do `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="9b06d-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="9b06d-106">Para obter mais informações sobre `mgt-person` o componente, consulte [docs-Person docs](./person.md).</span><span class="sxs-lookup"><span data-stu-id="9b06d-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="9b06d-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b06d-107">Example</span></span>

<span data-ttu-id="9b06d-108">O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="9b06d-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="9b06d-109">Passe o mouse sobre a pessoa para ver o cartão Person e use o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="9b06d-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="9b06d-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="9b06d-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="9b06d-111">Configuração para integrações do teams</span><span class="sxs-lookup"><span data-stu-id="9b06d-111">Setup for Teams integrations</span></span>

<span data-ttu-id="9b06d-112">O componente de cartão de pessoa permite que o usuário entre em contato com a pessoa de destino, incluindo via chat do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9b06d-112">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="9b06d-113">Se estiver usando o componente dentro de um aplicativo de guia do Teams, você pode garantir que o componente se vincule diretamente ao chat, em vez de `microsoftTeamsLib` abrir `TeamsProvider`uma janela do navegador, definindo o no.</span><span class="sxs-lookup"><span data-stu-id="9b06d-113">If using the component inside a Teams tab app, you can ensure that the component deep links directly to chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="9b06d-114">Se o componente de cartão de pessoa não conseguir detectar a biblioteca do Teams, o componente tentará abrir o cliente da Web do teams.</span><span class="sxs-lookup"><span data-stu-id="9b06d-114">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

<span data-ttu-id="9b06d-115">Para obter mais informações sobre `TeamsProvider` o provedor, consulte [Microsoft Teams Provider](../providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="9b06d-115">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9b06d-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b06d-116">Properties</span></span>

<span data-ttu-id="9b06d-117">O componente usa o Microsoft Graph para fornecer detalhes adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="9b06d-117">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="9b06d-118">Para definir um usuário, você deve usar a propriedade **Person-Query** de `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="9b06d-118">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="9b06d-119">Atributo</span><span class="sxs-lookup"><span data-stu-id="9b06d-119">Attribute</span></span>         | <span data-ttu-id="9b06d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b06d-120">Type</span></span>                     | <span data-ttu-id="9b06d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b06d-121">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="9b06d-122">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="9b06d-122">person-details</span></span> | <span data-ttu-id="9b06d-123">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="9b06d-123">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="9b06d-124">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="9b06d-124">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="9b06d-125">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="9b06d-125">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="9b06d-126">Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9b06d-126">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="9b06d-127">pessoa-imagem</span><span class="sxs-lookup"><span data-stu-id="9b06d-127">person-image</span></span>   | <span data-ttu-id="9b06d-128">png/jpg/SVG</span><span class="sxs-lookup"><span data-stu-id="9b06d-128">png/jpg/svg</span></span>                    | <span data-ttu-id="9b06d-129">Imagem relacionada à pessoa exibida no cartão.</span><span class="sxs-lookup"><span data-stu-id="9b06d-129">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="9b06d-130">Inherit-detalhes</span><span class="sxs-lookup"><span data-stu-id="9b06d-130">inherit-details</span></span>   | <span data-ttu-id="9b06d-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9b06d-131">None.</span></span>                  | <span data-ttu-id="9b06d-132">Permite que o cartão de pessoa percorra a `mgt-person` árvore pai para que o `person-details` componente `person-image` use o mesmo e os dados.</span><span class="sxs-lookup"><span data-stu-id="9b06d-132">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="9b06d-133">Modelos</span><span class="sxs-lookup"><span data-stu-id="9b06d-133">Templates</span></span>

<span data-ttu-id="9b06d-134">O componente de cartão de pessoa usa [modelos](../templates.md) que permitem que você adicione ou substitua partes do componente.</span><span class="sxs-lookup"><span data-stu-id="9b06d-134">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="9b06d-135">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="9b06d-135">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="9b06d-136">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="9b06d-136">Data type</span></span> | <span data-ttu-id="9b06d-137">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="9b06d-137">Data context</span></span> | <span data-ttu-id="9b06d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b06d-138">Description</span></span> |
| - | - | - |
| <span data-ttu-id="9b06d-139">sem dados</span><span class="sxs-lookup"><span data-stu-id="9b06d-139">no-data</span></span> | <span data-ttu-id="9b06d-140">null</span><span class="sxs-lookup"><span data-stu-id="9b06d-140">null</span></span> | <span data-ttu-id="9b06d-141">O modelo usado quando não há dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="9b06d-141">The template used when no data is available.</span></span>
| <span data-ttu-id="9b06d-142">Padrão.</span><span class="sxs-lookup"><span data-stu-id="9b06d-142">default</span></span> | <span data-ttu-id="9b06d-143">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="9b06d-143">`person`: The person details object</span></span> <br> <span data-ttu-id="9b06d-144">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="9b06d-144">`personImage`: The URL of the image</span></span> | <span data-ttu-id="9b06d-145">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="9b06d-145">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="9b06d-146">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="9b06d-146">person-details</span></span> | <span data-ttu-id="9b06d-147">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="9b06d-147">`person`: The person details object</span></span> | <span data-ttu-id="9b06d-148">O modelo usado para renderizar a parte superior do cartão Person.</span><span class="sxs-lookup"><span data-stu-id="9b06d-148">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="9b06d-149">contato-detalhes</span><span class="sxs-lookup"><span data-stu-id="9b06d-149">contact-details</span></span> | <span data-ttu-id="9b06d-150">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="9b06d-150">`person`: The person details object</span></span> | <span data-ttu-id="9b06d-151">O modelo usado para substituir a parte detalhes do contato do contêiner detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="9b06d-151">The template used to override the contact details part of the additional details container.</span></span> |
| <span data-ttu-id="9b06d-152">adicional-detalhes</span><span class="sxs-lookup"><span data-stu-id="9b06d-152">additional-details</span></span> | <span data-ttu-id="9b06d-153">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="9b06d-153">`person`: The person details object</span></span> <br> <span data-ttu-id="9b06d-154">`personImage`: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="9b06d-154">`personImage`: the URL of the image</span></span> | <span data-ttu-id="9b06d-155">O modelo usado para adicionar conteúdo personalizado ao contêiner detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="9b06d-155">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="9b06d-156">Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão.</span><span class="sxs-lookup"><span data-stu-id="9b06d-156">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
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

## <a name="css-custom-properties"></a><span data-ttu-id="9b06d-157">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="9b06d-157">CSS custom properties</span></span>

<span data-ttu-id="9b06d-158">O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="9b06d-158">The `mgt-person-card` component defines the following CSS custom properties.</span></span> <span data-ttu-id="9b06d-159">Para usar essas propriedades, você deve definir o seletor como o `mgt-person` elemento pai.</span><span class="sxs-lookup"><span data-stu-id="9b06d-159">To use these properties, you must define the selector as the parent `mgt-person` element.</span></span> 

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

<span data-ttu-id="9b06d-160">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="9b06d-160">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b06d-161">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b06d-161">Microsoft Graph permissions</span></span>

<span data-ttu-id="9b06d-162">Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="9b06d-162">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="9b06d-163">Autenticação</span><span class="sxs-lookup"><span data-stu-id="9b06d-163">Authentication</span></span>

<span data-ttu-id="9b06d-164">O controle de cartão de pessoa usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="9b06d-164">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="9b06d-165">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="9b06d-165">Extend for more control</span></span>

<span data-ttu-id="9b06d-166">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="9b06d-166">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="9b06d-167">Método</span><span class="sxs-lookup"><span data-stu-id="9b06d-167">Method</span></span> | <span data-ttu-id="9b06d-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b06d-168">Description</span></span> |
| - | - |
| <span data-ttu-id="9b06d-169">renderNoData</span><span class="sxs-lookup"><span data-stu-id="9b06d-169">renderNoData</span></span> | <span data-ttu-id="9b06d-170">Renderiza um estado quando nenhum dado de pessoa está disponível.</span><span class="sxs-lookup"><span data-stu-id="9b06d-170">Renders a state when no person data is available.</span></span> | 
| <span data-ttu-id="9b06d-171">renderPersonDetails</span><span class="sxs-lookup"><span data-stu-id="9b06d-171">renderPersonDetails</span></span> | <span data-ttu-id="9b06d-172">Renderiza o corpo principal do cartão de pessoa (imagem, nome, ícones).</span><span class="sxs-lookup"><span data-stu-id="9b06d-172">Renders the main body of the person card (image, name, icons).</span></span> |
| <span data-ttu-id="9b06d-173">renderPersonImage</span><span class="sxs-lookup"><span data-stu-id="9b06d-173">renderPersonImage</span></span> | <span data-ttu-id="9b06d-174">Renderiza a parte da imagem dos detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9b06d-174">Renders the image part of the person details.</span></span> |
| <span data-ttu-id="9b06d-175">renderPersonName</span><span class="sxs-lookup"><span data-stu-id="9b06d-175">renderPersonName</span></span> | <span data-ttu-id="9b06d-176">Renderiza a parte do nome dos detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9b06d-176">Renders the name part of the person details.</span></span> |
| <span data-ttu-id="9b06d-177">renderPersonTitle</span><span class="sxs-lookup"><span data-stu-id="9b06d-177">renderPersonTitle</span></span> | <span data-ttu-id="9b06d-178">Renderiza a parte de título dos detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9b06d-178">Renders the title part of the person details.</span></span> |
| <span data-ttu-id="9b06d-179">renderPersonSubtitle</span><span class="sxs-lookup"><span data-stu-id="9b06d-179">renderPersonSubtitle</span></span> | <span data-ttu-id="9b06d-180">Renderiza a parte do subtítulo dos detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9b06d-180">Renders the subtitle part of the person details.</span></span> |
| <span data-ttu-id="9b06d-181">renderContactIcons</span><span class="sxs-lookup"><span data-stu-id="9b06d-181">renderContactIcons</span></span> | <span data-ttu-id="9b06d-182">Renderiza a parte dos ícones de contato dos detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9b06d-182">Renders the contact icons part of the person details.</span></span> |
| <span data-ttu-id="9b06d-183">renderExpandedDetailsButton</span><span class="sxs-lookup"><span data-stu-id="9b06d-183">renderExpandedDetailsButton</span></span> | <span data-ttu-id="9b06d-184">Renderiza o botão para mostrar os detalhes expandidos.</span><span class="sxs-lookup"><span data-stu-id="9b06d-184">Renders the button to show the expanded details.</span></span> |
| <span data-ttu-id="9b06d-185">renderExpandedDetails</span><span class="sxs-lookup"><span data-stu-id="9b06d-185">renderExpandedDetails</span></span> | <span data-ttu-id="9b06d-186">Renderiza o conteúdo no contêiner de detalhes expandido.</span><span class="sxs-lookup"><span data-stu-id="9b06d-186">Renders the content in the expanded details container.</span></span> |
| <span data-ttu-id="9b06d-187">renderContactDetails</span><span class="sxs-lookup"><span data-stu-id="9b06d-187">renderContactDetails</span></span> | <span data-ttu-id="9b06d-188">Renderiza a parte dos detalhes do contato dos detalhes expandidos.</span><span class="sxs-lookup"><span data-stu-id="9b06d-188">Renders the contact details part of the expanded details.</span></span> |
| <span data-ttu-id="9b06d-189">renderAdditionalDetails</span><span class="sxs-lookup"><span data-stu-id="9b06d-189">renderAdditionalDetails</span></span> | <span data-ttu-id="9b06d-190">Renderiza a parte detalhes adicionais dos detalhes expandidos.</span><span class="sxs-lookup"><span data-stu-id="9b06d-190">Renders the additional details part of the expanded details.</span></span> |

