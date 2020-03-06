---
title: Tipo de recurso Contract
description: Representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7911d875f669e03a40cd9408e047b9f7d0aee0d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533007"
---
# <a name="contract-resource-type"></a>Tipo de recurso Contract

Namespace: Microsoft. Graph representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.

> **Importante:** Existe somente nos locatários do parceiro. Os locatários de parceiros são locatários do Azure AD que pertencem a parceiros da Microsoft que fazem parte do [provedor de soluções de nuvem da Microsoft](https://partnercenter.microsoft.com/en-us/partner/programs), da distribuição do Office 365 ou dos programas de parceria do Microsoft Advisor.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter contrato](../api/contract-get.md) | Contrato |Ler as propriedades de um objeto Contract específico. |
|[Listar contratos](../api/contract-list.md) | Coleção Contract | Lista de contratos no locatário do parceiro. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|ContractType|String|Tipo de contrato.<br><br>Os valores possíveis são:<br> *SyndicationPartner* -parceiro que revende exclusivamente e gerencia o O365 e o Intune para este cliente. Eles revendem e dão suporte a seus clientes.<br> *BreadthPartner* -o parceiro tem a capacidade de fornecer suporte administrativo para esse cliente. No entanto, o parceiro não tem permissão para revender para o cliente.<br>*ResellerPartner* -Partner que é semelhante a um parceiro de distribuição, exceto pelo fato de que o parceiro não tem acesso exclusivo a um locatário. No caso de distribuição, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.|
|Box|Guid|O identificador exclusivo do locatário do cliente referido por esta parceria. Corresponde à propriedade ID do recurso de organização do locatário do cliente. |
|DefaultDomainName|String|Uma cópia do nome de domínio padrão do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.|
|displayName|Cadeia de caracteres|Uma cópia do nome de exibição do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente for alterado.|
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
