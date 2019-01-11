---
title: tipo de recurso de iosSingleSignOnSettings
description: iOS configurações de autenticação Kerberos de single sign-on
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17c2e100f9762334173ca6ca7049d1e5933f8616
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841059"
---
# <a name="iossinglesignonsettings-resource-type"></a>tipo de recurso de iosSingleSignOnSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

iOS configurações de autenticação Kerberos de single sign-on
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAppsList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de identificadores de aplicativo que têm permissão para usar esse logon. Se esse campo for omitido, o login se aplica a todos os aplicativos no dispositivo. Esta coleção pode conter um máximo de 500 elementos.|
|allowedUrls|String collection|Lista das URLs de HTTP que deve coincidir para usar esse logon. Com o iOS 9.0 ou posterior, um caracteres curinga podem ser usadas.|
|displayName|Cadeia de caracteres|O nome de exibição das configurações de logon mostrado no dispositivo receptor.|
|kerberosPrincipalName|Cadeia de caracteres|Um nome UPN do Kerberos. Se não fornecido, o usuário é solicitado por um durante a instalação do perfil.|
|kerberosRealm|Cadeia de caracteres|Um nome de realm Kerberos. Maiusculas e minúsculas.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```





