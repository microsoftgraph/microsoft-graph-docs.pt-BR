---
title: Obter intuneBrandingProfile
description: Leia as propriedades e as relações do objeto intuneBrandingProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d4c5ab2227c1a63f434c42a38ed7169877e6bcd3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457437"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="ceb30-103">Obter intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="ceb30-103">Get intuneBrandingProfile</span></span>

<span data-ttu-id="ceb30-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ceb30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ceb30-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ceb30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ceb30-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ceb30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceb30-107">Leia as propriedades e as relações do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ceb30-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ceb30-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ceb30-108">Prerequisites</span></span>
<span data-ttu-id="ceb30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceb30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceb30-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceb30-111">Permission type</span></span>|<span data-ttu-id="ceb30-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ceb30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceb30-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceb30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ceb30-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ceb30-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ceb30-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceb30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceb30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceb30-116">Not supported.</span></span>|
|<span data-ttu-id="ceb30-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceb30-117">Application</span></span>|<span data-ttu-id="ceb30-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ceb30-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceb30-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceb30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ceb30-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ceb30-120">Optional query parameters</span></span>
<span data-ttu-id="ceb30-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ceb30-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ceb30-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb30-122">Request headers</span></span>
|<span data-ttu-id="ceb30-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceb30-123">Header</span></span>|<span data-ttu-id="ceb30-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ceb30-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceb30-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceb30-125">Authorization</span></span>|<span data-ttu-id="ceb30-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceb30-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceb30-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ceb30-127">Accept</span></span>|<span data-ttu-id="ceb30-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ceb30-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceb30-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb30-129">Request body</span></span>
<span data-ttu-id="ceb30-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ceb30-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceb30-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb30-131">Response</span></span>
<span data-ttu-id="ceb30-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceb30-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceb30-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceb30-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ceb30-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb30-134">Request</span></span>
<span data-ttu-id="ceb30-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceb30-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="ceb30-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb30-136">Response</span></span>
<span data-ttu-id="ceb30-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceb30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2095

{
  "value": {
    "@odata.type": "#microsoft.graph.intuneBrandingProfile",
    "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
    "profileName": "Profile Name value",
    "profileDescription": "Profile Description value",
    "isDefaultProfile": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "showDisplayNameNextToLogo": true,
    "themeColorLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "landingPageCustomizedImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "customPrivacyMessage": "Custom Privacy Message value",
    "isRemoveDeviceDisabled": true,
    "isFactoryResetDisabled": true,
    "companyPortalBlockedActions": [
      {
        "@odata.type": "microsoft.graph.companyPortalBlockedAction",
        "platform": "androidForWork",
        "ownerType": "company",
        "action": "remove"
      }
    ],
    "showAzureADEnterpriseApps": true,
    "showOfficeWebApps": true,
    "sendDeviceOwnershipChangePushNotification": true,
    "enrollmentAvailability": "availableWithoutPrompts",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```





