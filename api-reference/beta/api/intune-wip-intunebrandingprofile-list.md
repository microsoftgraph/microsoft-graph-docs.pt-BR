---
title: Listar intuneBrandingProfiles
description: Listar propriedades e relações dos objetos intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a67cffc0e64daff4edd7969b4326a3027e53da8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133819"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="c0be3-103">Listar intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="c0be3-103">List intuneBrandingProfiles</span></span>

<span data-ttu-id="c0be3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0be3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0be3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0be3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0be3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0be3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0be3-107">Listar propriedades e relações dos objetos [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0be3-107">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0be3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0be3-108">Prerequisites</span></span>
<span data-ttu-id="c0be3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0be3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0be3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0be3-111">Permission type</span></span>|<span data-ttu-id="c0be3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0be3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0be3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0be3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0be3-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0be3-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0be3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0be3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0be3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0be3-116">Not supported.</span></span>|
|<span data-ttu-id="c0be3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0be3-117">Application</span></span>|<span data-ttu-id="c0be3-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0be3-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0be3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0be3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c0be3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0be3-120">Request headers</span></span>
|<span data-ttu-id="c0be3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0be3-121">Header</span></span>|<span data-ttu-id="c0be3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0be3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0be3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0be3-123">Authorization</span></span>|<span data-ttu-id="c0be3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0be3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0be3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0be3-125">Accept</span></span>|<span data-ttu-id="c0be3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0be3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0be3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0be3-127">Request body</span></span>
<span data-ttu-id="c0be3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0be3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0be3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0be3-129">Response</span></span>
<span data-ttu-id="c0be3-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0be3-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0be3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0be3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0be3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0be3-132">Request</span></span>
<span data-ttu-id="c0be3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0be3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="c0be3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0be3-134">Response</span></span>
<span data-ttu-id="c0be3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0be3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




