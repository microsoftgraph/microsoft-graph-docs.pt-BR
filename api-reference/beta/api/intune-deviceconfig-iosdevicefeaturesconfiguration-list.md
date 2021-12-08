---
title: Listar iosDeviceFeaturesConfigurations
description: Listar propriedades e relações dos objetos iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c572d8b2469deb73d29314afd7454f001ce460e8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345279"
---
# <a name="list-iosdevicefeaturesconfigurations"></a>Listar iosDeviceFeaturesConfigurations

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos objetos [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8140

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
      "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "airPrintDestinations": [
        {
          "@odata.type": "microsoft.graph.airPrintDestination",
          "ipAddress": "Ip Address value",
          "resourcePath": "Resource Path value",
          "port": 4,
          "forceTls": true
        }
      ],
      "assetTagTemplate": "Asset Tag Template value",
      "contentFilterSettings": {
        "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
        "specificWebsitesOnly": [
          {
            "@odata.type": "microsoft.graph.iosBookmark",
            "url": "Url value",
            "bookmarkFolder": "Bookmark Folder value",
            "displayName": "Display Name value"
          }
        ],
        "websiteList": [
          {
            "@odata.type": "microsoft.graph.iosBookmark",
            "url": "Url value",
            "bookmarkFolder": "Bookmark Folder value",
            "displayName": "Display Name value"
          }
        ]
      },
      "lockScreenFootnote": "Lock Screen Footnote value",
      "homeScreenDockIcons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value",
                  "isWebClip": true
                }
              ]
            }
          ]
        }
      ],
      "homeScreenPages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenPage",
          "displayName": "Display Name value",
          "icons": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolder",
              "displayName": "Display Name value",
              "pages": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                  "displayName": "Display Name value",
                  "apps": [
                    {
                      "@odata.type": "microsoft.graph.iosHomeScreenApp",
                      "displayName": "Display Name value",
                      "bundleID": "Bundle ID value",
                      "isWebClip": true
                    }
                  ]
                }
              ]
            }
          ]
        }
      ],
      "homeScreenGridWidth": 3,
      "homeScreenGridHeight": 4,
      "notificationSettings": [
        {
          "@odata.type": "microsoft.graph.iosNotificationSettings",
          "bundleID": "Bundle ID value",
          "appName": "App Name value",
          "publisher": "Publisher value",
          "enabled": true,
          "showInNotificationCenter": true,
          "showOnLockScreen": true,
          "alertType": "banner",
          "badgesEnabled": true,
          "soundsEnabled": true,
          "previewVisibility": "alwaysShow"
        }
      ],
      "singleSignOnSettings": {
        "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
        "allowedAppsList": [
          {
            "@odata.type": "microsoft.graph.appListItem",
            "name": "Name value",
            "publisher": "Publisher value",
            "appStoreUrl": "https://example.com/appStoreUrl/",
            "appId": "App Id value"
          }
        ],
        "allowedUrls": [
          "Allowed Urls value"
        ],
        "displayName": "Display Name value",
        "kerberosPrincipalName": "Kerberos Principal Name value",
        "kerberosRealm": "Kerberos Realm value"
      },
      "wallpaperDisplayLocation": "lockScreen",
      "wallpaperImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "singleSignOnExtension": {
        "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
        "realm": "Realm value",
        "domains": [
          "Domains value"
        ],
        "blockAutomaticLogin": true,
        "cacheName": "Cache Name value",
        "credentialBundleIdAccessControlList": [
          "Credential Bundle Id Access Control List value"
        ],
        "domainRealms": [
          "Domain Realms value"
        ],
        "isDefaultRealm": true,
        "passwordBlockModification": true,
        "passwordExpirationDays": 6,
        "passwordExpirationNotificationDays": 2,
        "userPrincipalName": "User Principal Name value",
        "passwordRequireActiveDirectoryComplexity": true,
        "passwordPreviousPasswordBlockCount": 2,
        "passwordMinimumLength": 5,
        "passwordMinimumAgeDays": 6,
        "passwordRequirementsDescription": "Password Requirements Description value",
        "requireUserPresence": true,
        "activeDirectorySiteCode": "Active Directory Site Code value",
        "passwordEnableLocalSync": true,
        "blockActiveDirectorySiteAutoDiscovery": true,
        "passwordChangeUrl": "https://example.com/passwordChangeUrl/",
        "signInHelpText": "Sign In Help Text value",
        "managedAppsInBundleIdACLIncluded": true
      },
      "iosSingleSignOnExtension": {
        "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
        "realm": "Realm value",
        "domains": [
          "Domains value"
        ],
        "blockAutomaticLogin": true,
        "cacheName": "Cache Name value",
        "credentialBundleIdAccessControlList": [
          "Credential Bundle Id Access Control List value"
        ],
        "domainRealms": [
          "Domain Realms value"
        ],
        "isDefaultRealm": true,
        "passwordBlockModification": true,
        "passwordExpirationDays": 6,
        "passwordExpirationNotificationDays": 2,
        "userPrincipalName": "User Principal Name value",
        "passwordRequireActiveDirectoryComplexity": true,
        "passwordPreviousPasswordBlockCount": 2,
        "passwordMinimumLength": 5,
        "passwordMinimumAgeDays": 6,
        "passwordRequirementsDescription": "Password Requirements Description value",
        "requireUserPresence": true,
        "activeDirectorySiteCode": "Active Directory Site Code value",
        "passwordEnableLocalSync": true,
        "blockActiveDirectorySiteAutoDiscovery": true,
        "passwordChangeUrl": "https://example.com/passwordChangeUrl/",
        "signInHelpText": "Sign In Help Text value",
        "managedAppsInBundleIdACLIncluded": true
      }
    }
  ]
}
```




