---
title: tipo de recurso deviceManagementDerivedCredentialSettings
description: Entidade que descreve as configurações de nível de locatário para credenciais derivadas
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 06f87b7c2f94bcd95d27889bfb9ee0649c4aae92
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990019"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a>tipo de recurso deviceManagementDerivedCredentialSettings

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve as configurações de nível de locatário para credenciais derivadas

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementDerivedCredentialSettings](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Leia as propriedades e as relações do objeto [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .|
|[Atualizar deviceManagementDerivedCredentialSettings](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Atualiza as propriedades de um objeto [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a credencial derivada|
|helpUrl|String|A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.|
|displayName|String|O nome de exibição do perfil.|
|emissor|[deviceManagementDerivedCredentialIssuer](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|O provedor de credenciais derivado a ser usado. Os valores possíveis são: `intercede`, `entrustDatacard`, `purebred`.|
|notificationType|[deviceManagementDerivedCredentialNotificationType](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|Os métodos usados para informar ao usuário final para abrir o portal da empresa para entregar os perfis de Wi-Fi, VPN ou email que usam certificados para o dispositivo. Os valores possíveis são: `none`, `companyPortal`, `email`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```





