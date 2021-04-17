---
title: Tipo de recurso pkcs12Certificate
description: Representa a configuração para carregar um pkcs12Certificate.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 60350908901293ec9bf090c9e2bc174d70c922e5
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882380"
---
# <a name="pkcs12certificate-resource-type"></a>Tipo de recurso pkcs12Certificate

Namespace: microsoft.graph

Representa a configuração usada para carregar um certificado ao usar a autenticação de certificado de cliente HTTPS para chamar um ponto de extremidade do conector de API. A autenticação de certificado de cliente é uma autenticação mútua baseada em certificado, onde o cliente fornece um certificado de cliente para um ponto de extremidade da API para comprovar sua identidade. O certificado configurado de um conector de API é enviado pelo Azure AD para o ponto de extremidade da API determinado, que valida o certificado.

Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|pkcs12Value|Cadeia de caracteres| Representa o conteúdo pfx enviado. O valor deve ser uma versão codificada de base 64 do conteúdo real do certificado. Obrigatório.|
|password|String| A senha do arquivo pfx. Obrigatório. Se nenhuma senha for usada, você ainda deverá fornecer um valor `""` de .|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12Certificate"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.pkcs12Certificate",
  "pkcs12Value": "String",
  "password": "String"
}
```
