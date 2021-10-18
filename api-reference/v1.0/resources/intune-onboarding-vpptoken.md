---
title: Tipo de recurso vppToken
description: Você adquire várias licenças de aplicativos do iOS por meio do Apple Volume Purchase Program para Empresas ou Educação. Isso envolve configurar uma conta do Apple VPP do site da Apple e carregar o token do Apple VPP Empresarial ou Educacional ao Intune. Você pode sincronizar suas informações de volume de compras com o Intune e acompanhar o uso do aplicativo comprado por volume. Você pode carregar vários tokens do Apple VPP Empresarial ou Educacional.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f52e3bab37b4dd076a645d7e024762c4f80fbe4
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455636"
---
# <a name="vpptoken-resource-type"></a>Tipo de recurso vppToken

Namespace: microsoft.graph

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
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Estado atual do Token do Apple Volume Purchase Program. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Status atual de sincronização da última sincronização de aplicativo que foi feita usando o Token do Apple Volume Purchase Program. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Se os aplicativos para o token VPP serão automaticamente atualizados ou não.|
|countryOrRegion|Cadeia de caracteres|Se os aplicativos para o token VPP serão automaticamente atualizados.|

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
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```



