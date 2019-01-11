---
title: tipo de recurso de iosVppAppAssignedLicense
description: iOS atribuição de licença de Volume programa de compra. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
localization_priority: Normal
ms.openlocfilehash: 2264a83b7d0f5c5610a4a477ec9d1d33a6d943f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815569"
---
# <a name="iosvppappassignedlicense-resource-type"></a>tipo de recurso de iosVppAppAssignedLicense

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

iOS atribuição de licença de Volume programa de compra. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|coleção [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Lista as propriedades e os relacionamentos dos objetos [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Obter iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Leia as propriedades e os relacionamentos do objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Criar iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Crie um novo objeto de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Excluir iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-delete.md)|Nenhum|Exclui um [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[Atualizar iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Atualize as propriedades de um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userEmailAddress|Cadeia de caracteres|O endereço de email do usuário.|
|userId|Cadeia de caracteres|ID do usuário.|
|userName|Cadeia de caracteres|O nome de usuário.|
|userPrincipalName|Cadeia de caracteres|O nome da entidade de segurança do usuário.|

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





