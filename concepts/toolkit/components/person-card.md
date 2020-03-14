---
title: Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph
description: Um componente de cartão de pessoa é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 336e6beabc227a2574e41cf6a658d38fdabfcdcf
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639923"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph

Um componente de cartão de pessoa é um componente responsivo para exibir mais informações relacionadas a uma pessoa. Geralmente, é usado como um submenu do `mgt-person` componente.

Para obter mais informações sobre `mgt-person` o componente, consulte [docs-Person docs](./person.md).

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente. Passe o mouse sobre a pessoa para ver o cartão Person e use o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

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
| --- | --- | --- |
| Padrão. | `person`: O objeto de detalhes da pessoa <br> `personImage`: A URL da imagem | O modelo padrão substitui todo o componente pelo seu. |
| adicional-detalhes | `person`: O objeto de detalhes da pessoa <br> `personImage`: a URL da imagem | O modelo usado para adicionar conteúdo adicional ao cartão. |

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

O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

Para saber mais, confira [estilos de componentes](../style.md).

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões. 

## <a name="authentication"></a>Autenticação

O controle de cartão de pessoa usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md). 
