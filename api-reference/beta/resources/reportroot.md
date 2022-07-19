---
title: Tipo de recurso reportRoot
description: Representa um contêiner para recursos de relatório do Azure Active Directory (Azure AD).
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 51816aef9b5b21732111206785057233c5144bc5
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855935"
---
# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner para recursos de relatório do Azure Active Directory (Azure AD).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [coleção applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Recupere **objetos applicationSignInDetailedSummary** . |
| [Obter applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Leia as propriedades e as relações de um **objeto applicationSignInDetailedSummary** . |
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | Leia as propriedades e as relações de um **objeto applicationSignInSummary** . |
|[Listar credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md)|[Coleção credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Obtenha os detalhes dos objetos credentialUserRegistrationDetails para um determinado locatário.|
|[Listar userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[coleção userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Obtenha os objetos userCredentialUsageDetails para um determinado locatário. Os detalhes incluem informações do usuário, o status da redefinição e o motivo da falha.|
<!--Temporarily hide these functions until we document them and others.
|[getAzureADLicenseUsage](../api/reportroot-getazureadlicenseusage.md)|[azureADLicenseUsage](../resources/azureadlicenseusage.md) collection|**TODO: Add Description**|
|[getAzureADUserFeatureUsage](../api/reportroot-getazureaduserfeatureusage.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADFeatureUsage](../api/reportroot-getazureadfeatureusage.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md) collection|**TODO: Add Description**|
|[getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection|**TODO: Add Description**|
|[getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md)|[credentialUsageSummary](../resources/credentialusagesummary.md) collection|**TODO: Add -->

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|applicationSignInDetailedSummary|[coleção applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Representa um resumo detalhado de uma entrada de aplicativo.|
|authenticationMethods|[authenticationMethodsRoot](../resources/authenticationmethodsroot.md)|Contêiner para propriedades de navegação para Azure AD de métodos de autenticação.|
|credentialUserRegistrationDetails|[Coleção credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Detalhes do uso da redefinição de senha de autoatendimento e da MFA (autenticação multifator) para todos os usuários registrados.|
|userCredentialUsageDetails|[coleção userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Representa o uso de SSPR (redefinição de senha por autoatendimento) para um determinado locatário.|

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
