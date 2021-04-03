---
title: Tipo de recurso pkcs12Certificate
description: Representa a configuração para carregar um pkcs12Certificate em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f312a7be0bd29d57c1a6b7dc5c7e5d72e6d41206
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509367"
---
# <a name="pkcs12certificate-resource-type"></a>Tipo de recurso pkcs12Certificate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a configuração usada para **carregar um** certificado ao usar a autenticação de certificado de cliente HTTPS para chamar um ponto de extremidade do conector de API. A autenticação de certificado de cliente é uma autenticação mútua baseada em certificado, onde o cliente fornece um certificado de cliente para um ponto de extremidade da API para comprovar sua identidade. O certificado configurado de um conector de API é enviado pelo Azure AD para o ponto de extremidade da API determinado, que valida o certificado.

Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|pkcs12Value|Cadeia de caracteres| Este é o campo para o envio de conteúdo pfx. O valor deve ser uma versão codificada de base 64 do conteúdo real do certificado. Obrigatório.|
|password|String| Essa é a senha do arquivo pfx. Obrigatório. Se nenhuma senha for usada, ainda deverá fornecer um valor `""` de .|

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
