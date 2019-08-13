---
title: tipo de recurso iosVppAppAssignedLicense
description: atribuição de licença do programa de compra de volume iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8d2fa29557ce594d49b613e0101489cb810586c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366781"
---
# <a name="iosvppappassignedlicense-resource-type"></a>tipo de recurso iosVppAppAssignedLicense

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

atribuição de licença do programa de compra de volume iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|coleção [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Listar Propriedades e relações dos objetos [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Obter iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Leia as propriedades e as relações do objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Criar iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Criar um novo objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Excluir iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-delete.md)|Nenhum|Exclui [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[Atualizar iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Atualiza as propriedades de um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|useremailaddress|String|O endereço de email do usuário.|
|userId|String|A ID do usuário.|
|userName|Cadeia de caracteres|O nome de usuário.|
|userPrincipalName|String|O nome da entidade de segurança do usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```



