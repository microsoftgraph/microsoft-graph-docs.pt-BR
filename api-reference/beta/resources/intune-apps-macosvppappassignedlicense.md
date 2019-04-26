---
title: tipo de recurso macOsVppAppAssignedLicense
description: Atribuição de licença do programa de compra de volume MacOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31f8e078f7695a115ce92d6d3f687d41a13831fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553915"
---
# <a name="macosvppappassignedlicense-resource-type"></a>tipo de recurso macOsVppAppAssignedLicense

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de licença do programa de compra de volume MacOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|coleção [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Listar Propriedades e relações dos objetos [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Obter macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Leia as propriedades e as relações do objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Criar macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Criar um novo objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Excluir macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-delete.md)|Nenhum|Exclui [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).|
|[Atualizar macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Atualiza as propriedades de um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userEmailAddress|String|O endereço de email do usuário.|
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
  "@odata.type": "microsoft.graph.macOsVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





