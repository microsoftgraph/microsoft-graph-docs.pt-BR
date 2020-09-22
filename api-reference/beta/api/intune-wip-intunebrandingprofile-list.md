---
title: Listar Navegaçãointunebrandingprofiles
description: Listar Propriedades e relações dos objetos intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 830a460a212ef428f95571441907f8cc7745ceff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062453"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="429f8-103">Listar Navegaçãointunebrandingprofiles</span><span class="sxs-lookup"><span data-stu-id="429f8-103">List intuneBrandingProfiles</span></span>

<span data-ttu-id="429f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="429f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="429f8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="429f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="429f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="429f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="429f8-107">Listar Propriedades e relações dos objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="429f8-107">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="429f8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="429f8-108">Prerequisites</span></span>
<span data-ttu-id="429f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="429f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="429f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="429f8-111">Permission type</span></span>|<span data-ttu-id="429f8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="429f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="429f8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="429f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="429f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="429f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="429f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="429f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="429f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="429f8-116">Not supported.</span></span>|
|<span data-ttu-id="429f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="429f8-117">Application</span></span>|<span data-ttu-id="429f8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="429f8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="429f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="429f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="429f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="429f8-120">Request headers</span></span>
|<span data-ttu-id="429f8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="429f8-121">Header</span></span>|<span data-ttu-id="429f8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="429f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="429f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="429f8-123">Authorization</span></span>|<span data-ttu-id="429f8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="429f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="429f8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="429f8-125">Accept</span></span>|<span data-ttu-id="429f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="429f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="429f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="429f8-127">Request body</span></span>
<span data-ttu-id="429f8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="429f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="429f8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="429f8-129">Response</span></span>
<span data-ttu-id="429f8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="429f8-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="429f8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="429f8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="429f8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="429f8-132">Request</span></span>
<span data-ttu-id="429f8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="429f8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="429f8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="429f8-134">Response</span></span>
<span data-ttu-id="429f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="429f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2416

{
  "value": [
    {
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
      "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
      "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
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
      "disableClientTelemetry": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






