---
title: Tipo de recurso learningProvider
description: Representa uma entidade que contém os detalhes sobre um provedor de aprendizado.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: resourcePageType
ms.openlocfilehash: eb68ab517f0df414202ac8d676838fb3161472cf
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883254"
---
# <a name="learningprovider-resource-type"></a>Tipo de recurso learningProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entidade que contém os detalhes sobre um provedor de aprendizado no aprendizado do Viva.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar learningProviders](../api/employeeexperience-list-learningproviders.md)|[Coleção learningProvider](../resources/learningprovider.md)|Obtenha uma lista dos recursos [learningProvider](../resources/learningprovider.md) registrados no Aprendizagem do Viva para um locatário.|
|[Criar learningProvider](../api/employeeexperience-post-learningproviders.md)|[learningProvider](../resources/learningprovider.md)|Crie um novo [objeto learningProvider](../resources/learningprovider.md) e registre-o com Aprendizagem do Viva usando o nome de exibição e logotipos especificados para temas diferentes.|
|[Obter learningProvider](../api/learningprovider-get.md)|[learningProvider](../resources/learningprovider.md)|Leia as propriedades e as relações de um [objeto learningProvider](../resources/learningprovider.md) .|
|[Atualizar learningProvider](../api/learningprovider-update.md)|[learningProvider](../resources/learningprovider.md)|Atualize as propriedades de um [objeto learningProvider](../resources/learningprovider.md) .|
|[Excluir learningProvider](../api/employeeexperience-delete-learningproviders.md)|Nenhum|[Exclua um recurso learningProvider](../resources/learningprovider.md) e remova seu registro Aprendizagem do Viva para o locatário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição que aparece Aprendizagem do Viva. Obrigatório.|
|id|String|O identificador exclusivo do provedor de aprendizado. Obrigatório.|
|isEnabled|Booliano|O estado do provedor. Opcional.|
|loginWebUrl|Cadeia de caracteres|URL de autenticação para acessar os cursos do provedor. Opcional.|
|longLogoWebUrlForDarkTheme|Cadeia de caracteres|A URL do logotipo longo para o modo escuro, que precisa ser uma imagem publicamente acessível. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|
|longLogoWebUrlForLightTheme|String|A URL do logotipo longo para o modo claro, que precisa ser uma imagem publicamente acessível. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|
|squareLogoWebUrlForDarkTheme|Cadeia de caracteres|A URL do logotipo quadrado para o modo escuro, que precisa ser uma imagem acessível publicamente. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|
|squareLogoWebUrlForLightTheme|Cadeia de caracteres|A URL do logotipo quadrado para o modo claro, que precisa ser uma imagem publicamente acessível. Essa imagem seria salva no Armazenamento de Blobs do Aprendizagem do Viva para renderização no Aprendizagem do Viva aplicativo. Obrigatório.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|learningContents|[Coleção learningContent](../resources/learningcontent.md)|Itens de catálogo de aprendizagem para o provedor.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.learningProvider",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.learningProvider",
    "displayName": "String",
    "id": "String (identifier)",
    "isEnabled": "Boolean",
    "loginWebUrl": "String",
    "longLogoWebUrlForDarkTheme": "String",
    "longLogoWebUrlForLightTheme": "String",
    "squareLogoWebUrlForDarkTheme": "String",
    "squareLogoWebUrlForLightTheme": "String"
}
```

