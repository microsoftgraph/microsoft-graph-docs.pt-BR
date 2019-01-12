---
title: tipo de recurso de windowsAssignedAccessProfile
description: Perfil de acesso atribuído para Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 893e81e544286c6877b9443d96f610acb939e934
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972849"
---
# <a name="windowsassignedaccessprofile-resource-type"></a>tipo de recurso de windowsAssignedAccessProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Perfil de acesso atribuído para Windows.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsAssignedAccessProfiles](../api/intune-deviceconfig-windowsassignedaccessprofile-list.md)|coleção [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Lista as propriedades e os relacionamentos dos objetos [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|
|[Obter windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-get.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Leia as propriedades e os relacionamentos do objeto [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|
|[Criar windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-create.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Crie um novo objeto de [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|
|[Excluir windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-delete.md)|Nenhum|Exclui um [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).|
|[Atualizar windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-update.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Atualize as propriedades de um objeto [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|profileName|String|Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu Iniciar e os usuários aos quais essa configuração de quiosque é atribuída.|
|showTaskBar|Booliano|Essa configuração permite que o administrador especificar se a barra de tarefas é mostrada ou não.|
|appUserModelIds|String collection|Estes são os únicos repositório aplicativos do Windows que estarão disponíveis para início no menu Iniciar.|
|desktopAppPaths|String collection|Estes são os caminhos dos aplicativos de área de trabalho que estarão disponíveis no menu Iniciar e os aplicativos somente o usuário será capaz de início.|
|userAccounts|String collection|As contas de usuário que serão bloqueadas para esta configuração de quiosque.|
|startMenuLayoutXml|Binária|Permite que os administradores substituir o layout de início padrão e impede que o usuário alterá-la.O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout. XML deve estar em formato binário.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAssignedAccessProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "showTaskBar": true,
  "appUserModelIds": [
    "String"
  ],
  "desktopAppPaths": [
    "String"
  ],
  "userAccounts": [
    "String"
  ],
  "startMenuLayoutXml": "binary"
}
```





