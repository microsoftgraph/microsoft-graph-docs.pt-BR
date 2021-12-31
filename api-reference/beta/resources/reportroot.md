---
title: Tipo de recurso reportRoot
description: Contêiner para recursos de relatório do Azure AD.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0cd17a6f8a06b9c5a4b263b06c3bb3ec71d7dc0c
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647046"
---
# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner que expõe propriedades de navegação para recursos de relatório do Azure AD.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [Coleção applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Recuperar **objetos applicationSignInDetailedSummary.** |
| [Obter applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Leia as propriedades e as relações de um **objeto applicationSignInDetailedSummary.** |
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | Leia as propriedades e as relações de **um objeto applicationSignInSummary.** |
|[Listar credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md)|[coleção credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Obter os detalhes dos objetos credentialUserRegistrationDetails para um determinado locatário.|
|[Listar userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[Coleção userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Obter os objetos userCredentialUsageDetails para um determinado locatário. Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.|
<!--Temporarily hide these functions until we document them and others.
|[getAzureADLicenseUsage](../api/reportroot-getazureadlicenseusage.md)|[azureADLicenseUsage](../resources/azureadlicenseusage.md) collection|**TODO: Add Description**|
|[getAzureADUserFeatureUsage](../api/reportroot-getazureaduserfeatureusage.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADFeatureUsage](../api/reportroot-getazureadfeatureusage.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md) collection|**TODO: Add Description**|
|[getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection|**TODO: Add Description**|
|[getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md)|[credentialUsageSummary](../resources/credentialusagesummary.md) collection|**TODO: Add -->

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|applicationSignInDetailedSummary|[Coleção applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Representa um resumo detalhado de uma assinatura de aplicativo.|
|authenticationMethods|[authenticationMethodsRoot](../resources/authenticationmethodsroot.md)|Contêiner para propriedades de navegação para recursos de autenticação do Azure AD.|
|credentialUserRegistrationDetails|[coleção credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Detalhes do uso de redefinição de senha de autoatendados e autenticação multifafatória (MFA) para todos os usuários registrados.|
|userCredentialUsageDetails|[Coleção userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Representa o uso de redefinição de senha de autoatendados (SSPR) para um determinado locatário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot"
}
```
