---
title: Tipo de recurso vppToken
description: Você adquire várias licenças de aplicativos do iOS por meio do Apple Volume Purchase Program para Empresas ou Educação. Isso envolve configurar uma conta do Apple VPP do site da Apple e carregar o token do Apple VPP Empresarial ou Educacional ao Intune. Você pode sincronizar suas informações de volume de compras com o Intune e acompanhar o uso do aplicativo comprado por volume. Você pode carregar vários tokens do Apple VPP Empresarial ou Educacional.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3723be31160f6a6d884de97c03797e56afdfbc74
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046691"
---
# <a name="vpptoken-resource-type"></a>Tipo de recurso vppToken

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Você adquire várias licenças de aplicativos do iOS por meio do Apple Volume Purchase Program para Empresas ou Educação. Isso envolve configurar uma conta do Apple VPP do site da Apple e carregar o token do Apple VPP Empresarial ou Educacional ao Intune. Você pode sincronizar suas informações de volume de compras com o Intune e acompanhar o uso do aplicativo comprado por volume. Você pode carregar vários tokens do Apple VPP Empresarial ou Educacional.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar vppTokens](../api/intune-onboarding-vpptoken-list.md)|Coleção de [vppToken](../resources/intune-onboarding-vpptoken.md)|Listar propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Obter vppToken](../api/intune-onboarding-vpptoken-get.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Ler propriedades e relações do objeto [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Criar vppToken](../api/intune-onboarding-vpptoken-create.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Criar um novo objeto [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Excluir vppToken](../api/intune-onboarding-vpptoken-delete.md)|Nenhum|Exclui um [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[Atualizar vppToken](../api/intune-onboarding-vpptoken-update.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Atualizar as propriedades de um objeto de [vppToken](../resources/intune-onboarding-vpptoken.md).|
|[ação syncLicenses](../api/intune-onboarding-vpptoken-synclicenses.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico|
|[ação revokeLicenses](../api/intune-onboarding-vpptoken-revokelicenses.md)|Nenhum|Revogar licenças associadas a uma appleVolumePurchaseProgramToken específica|
|[Função getLicensesForApp](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|[Coleção vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)|Ainda não documentado|
|[Ação syncLicenseCounts](../api/intune-onboarding-vpptoken-synclicensecounts.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado. É a Chave da entidade.|
|organizationName|Cadeia de caracteres|A organização associada ao Token do Programa de Compra por Volume da Apple|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado. Os valores possíveis são: `business`, `education`. Os valores possíveis são: `business`, `education`.|
|appleId|Cadeia de caracteres|O Apple ID associado ao Token do Apple Volume Purchase Program.|
|expirationDateTime|DateTimeOffset|A data e hora de expiração do Token do Apple Volume Purchase Program.|
|lastSyncDateTime|DateTimeOffset|A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando o Token do Apple Volume Purchase Program.|
|token|Cadeia de caracteres|A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Estado atual do Token do Apple Volume Purchase Program. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Os possíveis valores são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`, `duplicateLocationId`.|
|tokenActionResults|[Coleção vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|A coleção de status das ações executadas no Token do Programa de Compra de Volume da Apple.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Se os aplicativos para o token VPP serão automaticamente atualizados ou não.|
|countryOrRegion|Cadeia de caracteres|Se os aplicativos para o token VPP serão automaticamente atualizados ou não.|
|dataSharingConsentGranted|Boleano|Consentimento concedido para compartilhamento de dados com o Programa de Compra de Volume da Apple.|
|displayName|Cadeia de caracteres|Um nome amigável de token especificado pelo administrador.|
|locationName|Cadeia de Caracteres|Local do token retornado do VPP da Apple.|
|claimTokenManagementFromExternalMdm|Boleano|Consentimento do administrador para permitir o gerenciamento de token de declaração do MDM externo.|
|roleScopeTagIds|String collection|IDs de marcas de escopo de função atribuídas a essa entidade.|

## <a name="relationships"></a>Relações
Nenhum

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



