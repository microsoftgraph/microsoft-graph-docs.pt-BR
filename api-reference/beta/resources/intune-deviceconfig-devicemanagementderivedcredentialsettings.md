---
title: tipo de recurso deviceManagementDerivedCredentialSettings
description: Entidade que descreve as configurações de nível de locatário para credenciais derivadas
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fa7adfa76482cd4c67c2c3faaaf96b760f44bd2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33956885"
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
|id|Cadeia de caracteres|Identificador exclusivo para a credencial derivada|
|helpUrl|Cadeia de caracteres|A URL que será acessível aos usuários finais à medida que eles recuperarem uma credencial derivada usando o portal da empresa.|
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




