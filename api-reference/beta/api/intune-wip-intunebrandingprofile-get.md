---
title: Obter intuneBrandingProfile
description: Leia as propriedades e as relações do objeto intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2915b03d1dc850ee854f0b696a54efe109fd60c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458168"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="450ff-103">Obter intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="450ff-103">Get intuneBrandingProfile</span></span>

<span data-ttu-id="450ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="450ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="450ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="450ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="450ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="450ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="450ff-107">Leia as propriedades e as relações do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="450ff-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="450ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="450ff-108">Prerequisites</span></span>
<span data-ttu-id="450ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="450ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="450ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="450ff-111">Permission type</span></span>|<span data-ttu-id="450ff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="450ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="450ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="450ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="450ff-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="450ff-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="450ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="450ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="450ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="450ff-116">Not supported.</span></span>|
|<span data-ttu-id="450ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="450ff-117">Application</span></span>|<span data-ttu-id="450ff-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="450ff-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="450ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="450ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="450ff-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="450ff-120">Optional query parameters</span></span>
<span data-ttu-id="450ff-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="450ff-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="450ff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="450ff-122">Request headers</span></span>
|<span data-ttu-id="450ff-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="450ff-123">Header</span></span>|<span data-ttu-id="450ff-124">Valor</span><span class="sxs-lookup"><span data-stu-id="450ff-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="450ff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="450ff-125">Authorization</span></span>|<span data-ttu-id="450ff-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="450ff-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="450ff-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="450ff-127">Accept</span></span>|<span data-ttu-id="450ff-128">application/json</span><span class="sxs-lookup"><span data-stu-id="450ff-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="450ff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="450ff-129">Request body</span></span>
<span data-ttu-id="450ff-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="450ff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="450ff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="450ff-131">Response</span></span>
<span data-ttu-id="450ff-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="450ff-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="450ff-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="450ff-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="450ff-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="450ff-134">Request</span></span>
<span data-ttu-id="450ff-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="450ff-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="450ff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="450ff-136">Response</span></span>
<span data-ttu-id="450ff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="450ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



