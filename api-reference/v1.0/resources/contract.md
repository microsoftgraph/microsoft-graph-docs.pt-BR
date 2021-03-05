---
title: Tipo de recurso de contrato
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 35e8cbc38fd183907c09b26c05d5c95cc140a7f5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444424"
---
# <a name="contract-resource-type"></a>Tipo de recurso de contrato

Namespace: microsoft.graph Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.

> **Importante:** Existe apenas em locatários parceiros. Os locatários de parceiros são locatários do Azure AD que pertencem aos parceiros da Microsoft que fazem parte do [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), do Office 365 Syndication ou dos programas de parceiros do Microsoft Advisor.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter contrato](../api/contract-get.md) | Contrato |Ler propriedades de um objeto de contrato específico. |
|[Listar contratos](../api/contract-list.md) | Coleção Contract | Lista de contratos no locatário do parceiro. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|contractType|Cadeia de caracteres|Tipo de contrato.<br><br>Os valores possíveis são:<br> *SyndicationPartner* - Parceiro que revende e gerencia exclusivamente o O365 e o Intune para esse cliente. Eles revendem e suportam seus clientes.<br> *BreadthPartner* - O parceiro tem a capacidade de fornecer suporte administrativo para esse cliente. No entanto, o parceiro não tem permissão para revender para o cliente.<br>*ResellerPartner* - Parceiro semelhante a um parceiro de sindicalidade, exceto que o parceiro não tem acesso exclusivo a um locatário. No caso de sindicalização, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.|
|customerId|Guid|O identificador exclusivo do locatário do cliente referenciado por essa parceria. Corresponde à propriedade id do recurso de organização do locatário do cliente. |
|defaultDomainName|Cadeia de caracteres|Uma cópia do nome de domínio padrão do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente mudar.|
|displayName|Cadeia de caracteres|Uma cópia do nome de exibição do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente mudar.|
|id|Cadeia de caracteres| O identificador exclusivo da parceria. Chave, somente leitura |

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

