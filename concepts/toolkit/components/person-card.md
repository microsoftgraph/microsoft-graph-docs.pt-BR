---
title: Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph
description: Um componente de cartão de pessoa é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: f4d8c975fe91d91658f512cea708ee104d4fd906
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275854"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph

Um componente de cartão de pessoa é um componente responsivo para exibir mais informações relacionadas a uma pessoa. Geralmente, é usado como um submenu do `mgt-person` componente.

Para obter mais informações sobre `mgt-person` o componente, consulte [docs-Person docs](./person.md).
  
## <a name="example"></a>Exemplo

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a>Propriedades

O componente usa o Microsoft Graph para fornecer detalhes adicionais sobre o usuário. Para definir um usuário, você deve usar a propriedade **Person-Query** de `mgt-person`.

| Atributo         | type                     | Descrição                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| pessoa-detalhes | MicrosoftGraph. User <br> MicrosoftGraph. Person <br> MicrosoftGraph. Contact | Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário. |
| pessoa-imagem   | png/jpg/SVG                    | Imagem relacionada à pessoa exibida no cartão.                                   |



## <a name="templates"></a>Modelos

O componente de cartão de pessoa usa [modelos](../templates.md) que permitem que você adicione ou substitua partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | Person: o objeto de detalhes da pessoa <br> personImage: a URL da imagem | O modelo padrão substitui todo o componente pelo seu. |
| adicional-detalhes | Person: o objeto de detalhes da pessoa <br> personImage: a URL da imagem | O modelo usado para adicionar conteúdo adicional ao cartão. |

Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão. 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card person-details="{{person}}" 
            person-image="{{personImage}}">
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
