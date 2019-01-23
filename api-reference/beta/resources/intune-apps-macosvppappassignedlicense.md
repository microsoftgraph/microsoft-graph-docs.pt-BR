---
title: tipo de recurso de macOsVppAppAssignedLicense
description: Atribuição de licença do programa de compras MacOS Volume. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c3a029d0f0aca7ab295f34d108b8bf61bdc17dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429033"
---
# <a name="macosvppappassignedlicense-resource-type"></a>tipo de recurso de macOsVppAppAssignedLicense

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atribuição de licença do programa de compras MacOS Volume. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|coleção [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Lista as propriedades e os relacionamentos dos objetos [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Obter macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Leia as propriedades e os relacionamentos do objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Criar macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Crie um novo objeto de [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Excluir macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-delete.md)|Nenhum|Exclui um [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).|
|[Atualizar macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Atualize as propriedades de um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|userEmailAddress|String|O endereço de email do usuário.|
|userId|String|ID do usuário.|
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




