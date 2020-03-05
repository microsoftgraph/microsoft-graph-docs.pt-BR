---
title: tipo de recurso trustFrameworkKeySet
description: Representa um conjunto de chaves/diretivas de política de confiança.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2620a7aca90e8a8ae27880343914dfcbbabe27d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519642"
---
# <a name="trustframeworkkeyset-resource-type"></a>tipo de recurso trustFrameworkKeySet

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de chaves/diretivas de política de confiança. A estrutura de experiência de identidade armazena os segredos, que podem ser usados nas políticas. Os segredos podem ser senhas, certificados ou outros arquivos. No portal, essas entidades são mostradas como `Policy keys`. A estrutura de experiência de identidade usa o padrão JWK (JSON Web Key) para os conjuntos de chaves. Esta entidade segue o formato especificado na [RFC 7517 seção 5](https://tools.ietf.org/html/rfc7517#section-5).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/trustframework-list-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) Coletânea | Listar trustFrameworkKeySets. |
| [Create](../api/trustframework-post-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Criar trustFrameworkKeySet. |
| [Get](../api/trustframeworkkeyset-get.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Leia as propriedades e os relacionamentos do objeto trustFrameworkKeySet. |
| [Update](../api/trustframeworkkeyset-update.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Atualize o objeto trustFrameworkKeySet. |
| [Delete](../api/trustframeworkkeyset-delete.md) | None | Exclua o objeto trustFrameworkKeySet. |
|[Gerar chave](../api/trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Gerar uma chave no conjunto de chaves. |
|[Obter chave ativa](../api/trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Obtém a chave ativa atualmente no conjunto de chaves. |
|[Carregar certificado](../api/trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](trustframeworkkey.md)| Carregar um certificado X. 509. |
|[Carregar PKCS12](../api/trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](trustframeworkkey.md)| Carregar um certificado no formato PKCS12. |
|[Carregar segredo](../api/trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](trustframeworkkey.md)| Carregar um segredo baseado em cadeia de caracteres. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo do conjunto de chaves trustframework |
|as|coleção [trustFrameworkKey](trustframeworkkey.md)| Uma coleção das chaves. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "baseType": "",
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
