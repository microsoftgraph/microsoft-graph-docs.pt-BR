---
title: Tipo de recurso vppToken
description: Você adquire várias licenças de aplicativos do iOS por meio do Apple Volume Purchase Program para Empresas ou Educação. Isso envolve configurar uma conta do Apple VPP do site da Apple e carregar o token do Apple VPP Empresarial ou Educacional ao Intune. Você pode sincronizar suas informações de volume de compras com o Intune e acompanhar o uso do aplicativo comprado por volume. Você pode carregar vários tokens do Apple VPP Empresarial ou Educacional.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 806c652e7d1d75de16dd40f4db1dfc39ae4f442a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774117"
---
# <a name="vpptoken-resource-type"></a>Tipo de recurso vppToken

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Você adquire várias licenças de aplicativos do iOS por meio do Apple Volume Purchase Program para Empresas ou Educação. Isso envolve configurar uma conta do Apple VPP do site da Apple e carregar o token do Apple VPP Empresarial ou Educacional ao Intune. Você pode sincronizar suas informações de volume de compras com o Intune e acompanhar o uso do aplicativo comprado por volume. Você pode carregar vários tokens do Apple VPP Empresarial ou Educacional.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar vppTokens](../api/intune-onboarding-vpptoken-list.md)|Coleção de [vppToken](../resources/intune-onboarding-vpptoken.md)|Listar propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Obter vppToken](../api/intune-onboarding-vpptoken-get.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Ler propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Criar vppToken](../api/intune-onboarding-vpptoken-create.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Criar um novo objeto [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Excluir vppToken](../api/intune-onboarding-vpptoken-delete.md)|Nenhum|Exclui um [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Atualizar vppToken](../api/intune-onboarding-vpptoken-update.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Atualizar as propriedades de um objeto [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[ação syncLicenses](../api/intune-onboarding-vpptoken-synclicenses.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico|
|[ação revokeLicenses](../api/intune-onboarding-vpptoken-revokelicenses.md)|Nenhum|Revogar licenças associadas a um determinado appleVolumePurchaseProgramToken|
|[função getLicensesForApp](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|coleção [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado. É a Chave da entidade.|
|organizationName|String|A organização associada ao Token do Programa de Compra por Volume da Apple|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado. Os valores possíveis são: `business` e `education`. Os valores possíveis são: `business`, `education`.|
|appleId|Cadeia de caracteres|O Apple ID associado ao Token do Apple Volume Purchase Program.|
|expirationDateTime|DateTimeOffset|A data e hora de expiração do Token do Apple Volume Purchase Program.|
|lastSyncDateTime|DateTimeOffset|A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.|
|token|Cadeia de caracteres|A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Estado atual do Token do Apple Volume Purchase Program. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|tokenActionResults|coleção [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|A coleção de status das ações executadas no token do Apple Volume Purchase Program.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Se os aplicativos para o token VPP serão automaticamente atualizados ou não.|
|countryOrRegion|Cadeia de caracteres|Se os aplicativos para o token VPP serão automaticamente atualizados ou não.|
|dataSharingConsentGranted|Booliano|Consentimento concedido para compartilhamento de dados com o Apple Volume Purchase Program.|
|displayName|Cadeia de caracteres|Um nome amigável de token especificado pelo administrador.|
|LocationName|Cadeia de caracteres|Local do token retornado da Apple VPP.|
|claimTokenManagementFromExternalMdm|Booliano|Consentimento do administrador para permitir o reivindicação de gerenciamento de token de MDM externo.|
|roleScopeTagIds|Coleção String|IDs de marcas de escopo de função atribuídas a esta entidade.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String",
  "dataSharingConsentGranted": true,
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```





