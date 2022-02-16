---
title: Tipo de recurso de contrato
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e872f2f102f9b906e55e917efdc80d50135c3514
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854554"
---
# <a name="contract-resource-type"></a>Tipo de recurso de contrato

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.

> **Importante:** Existe apenas em locatários parceiros. Os locatários de parceiros são locatários do Azure AD que pertencem aos parceiros da Microsoft que fazem parte dos programas de parceiros [Provedor de Soluções na Nuvem da Microsoft, Office 365](https://partnercenter.microsoft.com/partner/programs) Syndication ou Microsoft Advisor.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter contrato](../api/contract-get.md) | Contrato |Ler propriedades de um objeto de contrato específico. |
|[Listar contratos](../api/contract-list.md) | Coleção Contract | Lista de contratos no locatário do parceiro. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|contractType|Cadeia de caracteres|Tipo de contrato. Os valores possíveis são:  `SyndicationPartner`, `BreadthPartner`, `ResellerPartner`. Confira mais na [tabela abaixo](#contracttype-values). |
|customerId|GUID|O identificador exclusivo do locatário do cliente referenciado por essa parceria. Corresponde à propriedade id do recurso de organização do locatário do cliente. |
|defaultDomainName|String|Uma cópia do nome de domínio padrão do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente mudar.|
|displayName|Cadeia de caracteres|Uma cópia do nome de exibição do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente mudar.|
|id|String| O identificador exclusivo da parceria. Chave, somente leitura |

### <a name="contracttype-values"></a>valores contractType

|Member|Descrição|
|:---|:---|
|SyndicationPartner|Parceiro que *revende* e gerencia exclusivamente o O365 e o Intune para esse cliente. Eles revendem e suportam seus clientes.|
|BreadthPartner|O parceiro tem a capacidade de fornecer suporte administrativo para esse cliente. No entanto, o parceiro não tem permissão para revender para o cliente.|
|ResellerPartner|Parceiro semelhante a um parceiro de sindicalidade, exceto que o parceiro não tem acesso exclusivo a um locatário. No caso de sindicalização, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "GUID",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


