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
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph

Um componente de cartão de pessoa é um componente responsivo para exibir mais informações relacionadas a uma pessoa. Geralmente, é usado como um submenu do `mgt-person` componente.

Para obter mais informações sobre `mgt-person` o componente, consulte [docs-Person docs](./person.md).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente. Passe o mouse sobre a pessoa para ver o cartão Person e use o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="setup-for-teams-integrations"></a>Configuração para integrações do teams

O componente de cartão de pessoa permite que o usuário entre em contato com a pessoa de destino, incluindo via chat do Microsoft Teams. Se estiver usando o componente dentro de um aplicativo de guia do Teams, você pode garantir que o componente se vincule diretamente ao chat, em vez de `microsoftTeamsLib` abrir `TeamsProvider`uma janela do navegador, definindo o no.

Se o componente de cartão de pessoa não conseguir detectar a biblioteca do Teams, o componente tentará abrir o cliente da Web do teams.

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

Para obter mais informações sobre `TeamsProvider` o provedor, consulte [Microsoft Teams Provider](../providers/teams.md).

## <a name="properties"></a>Propriedades

O componente usa o Microsoft Graph para fornecer detalhes adicionais sobre o usuário. Para definir um usuário, você deve usar a propriedade **Person-Query** de `mgt-person`.

| Atributo         | Tipo                     | Descrição                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| pessoa-detalhes | MicrosoftGraph. User <br> MicrosoftGraph. Person <br> MicrosoftGraph. Contact | Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário. |
| pessoa-imagem   | png/jpg/SVG                    | Imagem relacionada à pessoa exibida no cartão.                                   |
| Inherit-detalhes   | Nenhum.                  | Permite que o cartão de pessoa percorra a `mgt-person` árvore pai para que o `person-details` componente `person-image` use o mesmo e os dados.                      |


## <a name="templates"></a>Modelos

O componente de cartão de pessoa usa [modelos](../templates.md) que permitem que você adicione ou substitua partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| - | - | - |
| sem dados | null | O modelo usado quando não há dados disponíveis.
| Padrão. | `person`: O objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo padrão substitui todo o componente pelo seu. |
| pessoa-detalhes | `person`: O objeto de detalhes da pessoa | O modelo usado para renderizar a parte superior do cartão Person. |
| contato-detalhes | `person`: O objeto de detalhes da pessoa | O modelo usado para substituir a parte detalhes do contato do contêiner detalhes adicionais. |
| adicional-detalhes | `person`: O objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo usado para adicionar conteúdo personalizado ao contêiner detalhes adicionais. |

Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão. 

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

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS. Para usar essas propriedades, você deve definir o seletor como o `mgt-person` elemento pai. 

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

Para saber mais, confira [estilos de componentes](../style.md).

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões. 

## <a name="authentication"></a>Autenticação

O controle de cartão de pessoa usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md). 

## <a name="extend-for-more-control"></a>Estender para mais controle

Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.

| Método | Descrição |
| - | - |
| renderNoData | Renderiza um estado quando nenhum dado de pessoa está disponível. | 
| renderPersonDetails | Renderiza o corpo principal do cartão de pessoa (imagem, nome, ícones). |
| renderPersonImage | Renderiza a parte da imagem dos detalhes da pessoa. |
| renderPersonName | Renderiza a parte do nome dos detalhes da pessoa. |
| renderPersonTitle | Renderiza a parte de título dos detalhes da pessoa. |
| renderPersonSubtitle | Renderiza a parte do subtítulo dos detalhes da pessoa. |
| renderContactIcons | Renderiza a parte dos ícones de contato dos detalhes da pessoa. |
| renderExpandedDetailsButton | Renderiza o botão para mostrar os detalhes expandidos. |
| renderExpandedDetails | Renderiza o conteúdo no contêiner de detalhes expandido. |
| renderContactDetails | Renderiza a parte dos detalhes do contato dos detalhes expandidos. |
| renderAdditionalDetails | Renderiza a parte detalhes adicionais dos detalhes expandidos. |

