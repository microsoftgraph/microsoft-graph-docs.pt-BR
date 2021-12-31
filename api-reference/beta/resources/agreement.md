---
title: tipo de recurso de contrato
description: Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 28abdafb3adda1b1fd3356fcdd1db5bda86c804f
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651376"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o recurso Azure Active Directory [termos de uso](/azure/active-directory/conditional-access/terms-of-use) de acordo com seu cenário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar acordos](../api/termsofusecontainer-post-agreements.md) | [agreement](agreement.md) | Crie um novo contrato postando na coleção de contratos. |
| [Listar contratos](../api/termsofusecontainer-list-agreements.md) | [coleção agreement](agreement.md) | Obter uma coleção de objetos de contrato. |
| [Obter contrato](../api/agreement-get.md) | [agreement](agreement.md) | Ler propriedades e relações de um objeto de contrato. |
| [Atualizar contrato](../api/agreement-update.md) | [agreement](agreement.md) | Atualize um objeto agreement. |
| [Excluir contrato](../api/agreement-delete.md) | Nenhum | Excluir um objeto agreement. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String|Nome de exibição do contrato. O nome de exibição é usado para o controle interno do contrato, mas não é mostrado aos usuários finais que visualizam o contrato.|
|id|String| Somente leitura.|
|isPerDeviceAcceptanceRequired|Booliano|Essa configuração permite exigir que os usuários finais aceitem esse contrato em todos os dispositivos de onde eles estão acessando. O usuário final será necessário para registrar seu dispositivo no Azure AD, caso ainda não tenha feito isso.|
|isViewingBeforeAcceptanceRequired|Booliano|Indica se o usuário precisa expandir o contrato antes de aceitar.|
|termsExpiration|[termsExpiration](termsexpiration.md)| Cronograma de expiração e frequência de acordo para todos os usuários. |
|userReacceptRequiredFrequency|Duração|A duração após a qual o usuário deve aceitar os termos de uso. O valor é representado no formato ISO 8601 por durações.|


## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|acceptances|Coleção [agreementAcceptance](agreementacceptance.md)|Somente leitura. Informações sobre as aceitaçãos deste contrato.|
|file|[agreementFile](agreementfile.md) | PDF padrão vinculado a este contrato.|
|arquivos|[Coleção agreementFileLocalization](agreementfilelocalization.md)| PDFs vinculados a este contrato. **Observação:** Essa propriedade está em processo de preterido. Use a  **propriedade file** em vez disso.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "String (identifier)",
  "displayName": "String",
  "termsExpiration": {
    "@odata.type": "microsoft.graph.termsExpiration"
  },
  "userReacceptRequiredFrequency": "String (duration)",
  "isViewingBeforeAcceptanceRequired": "Boolean",
  "isPerDeviceAcceptanceRequired": "Boolean"
}
```
