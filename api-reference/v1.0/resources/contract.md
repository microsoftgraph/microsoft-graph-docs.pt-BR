---
title: Tipo de recurso contact
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
localization_priority: Normal
ms.openlocfilehash: c14f4a51cbab5625c16ef0f0e515fffd35619366
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812296"
---
# <a name="contract-resource-type"></a>Tipo de recurso contact
Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.

> **Importante:** Existe apenas em locatários do parceiro. Locatários do parceiro são locatários Azure AD que pertencem a parceiros da Microsoft que fazem parte do [Provedor de Soluções do Microsoft Cloud](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication ou programas de parceiro Microsoft Advisor.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Get contract](../api/contract-get.md) | Contrato |Ler propriedades de um objeto de contrato específico. |
|[List contracts](../api/contract-list.md) | Coleção de contratos | Lista de contratos no locatário parceiro. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|contractType|String|Tipo de contrato.<br><br>Os valores possíveis são:<br> *SyndicationPartner* – parceiro que revende ou gerencia com exclusividade O365 e Intune para esse cliente. Eles revendem e oferecem suporte aos seus clientes.<br> *BreadthPartner* – parceiro tem a capacidade de fornecer suporte administrativo para esse cliente. No entanto, o parceiro não tem permissão para revender ao cliente.<br>*ResellerPartner* – parceiro que é semelhante a um parceiro de agregação, exceto que o parceiro não tem acesso exclusivo ao locatário. No caso de agregação, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.|
|customerId|Guid|O identificador exclusivo para o locatário de cliente referenciado por essa parceria. Corresponde à propriedade de identificação do recurso de organização do locatário do cliente. |
|defaultDomainName|String|Uma cópia do nome de domínio padrão do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.|
|displayName|String|Uma cópia do nome de exibição do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de exibição do locatário do cliente é alterado.|
|id|String| O identificador exclusivo da parceria. Chave, somente leitura |

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
