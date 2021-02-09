---
title: Tipo de recurso trustFrameworkKeySet
description: Representa um keyset/policy da estrutura de confiança.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4223681a11ff11b8ea75b165247b5269d1a6cf84
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159847"
---
# <a name="trustframeworkkeyset-resource-type"></a>Tipo de recurso trustFrameworkKeySet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um keyset/policy da estrutura de confiança. A estrutura da Experiência de Identidade armazena os segredos, que podem ser usados nas políticas. Os segredos podem ser senhas, certificados ou outros arquivos. No portal, essas entidades são mostradas como `Policy keys` . A estrutura Identity Experience usa o padrão JWK (JWK) JSON para os keysets. Esta entidade segue o formato especificado na [RFC 7517 Seção 5](https://tools.ietf.org/html/rfc7517#section-5).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/trustframework-list-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) Coleção | Listar trustFrameworkKeySets. |
| [Criar](../api/trustframework-post-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Crie trustFrameworkKeySet. |
| [Get](../api/trustframeworkkeyset-get.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Leia as propriedades e os relacionamentos do objeto trustFrameworkKeySet. |
| [Update](../api/trustframeworkkeyset-update.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Atualize o objeto trustFrameworkKeySet. |
| [Delete](../api/trustframeworkkeyset-delete.md) | Nenhum(a) | Exclua o objeto trustFrameworkKeySet. |
|[Gerar chave](../api/trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Gere uma chave no keyset. |
|[Obter chave ativa](../api/trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Obter a chave ativa no momento no keyset. |
|[Carregar certificado](../api/trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](trustframeworkkey.md)| Carregar um certificado X.509. |
|[Carregar PKCS12](../api/trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](trustframeworkkey.md)| Carregar um certificado de formato PKCS12. |
|[Carregar segredo](../api/trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](trustframeworkkey.md)| Carregar um segredo baseado em cadeia de caracteres. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo do keyset trustframework |
|teclas|[Coleção trustFrameworkKey](trustframeworkkey.md)| Uma coleção de chaves. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "keys": [{"@odata.type": "microsoft.graph.trustFrameworkKey"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


