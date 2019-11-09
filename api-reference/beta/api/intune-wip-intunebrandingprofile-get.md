---
title: Obter intuneBrandingProfile
description: Leia as propriedades e as relações do objeto intuneBrandingProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbfe8484bf7dc877fc6e0745c26768a3dd8963bf
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087955"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="4abf0-103">Obter intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="4abf0-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="4abf0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4abf0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4abf0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4abf0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4abf0-106">Leia as propriedades e as relações do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4abf0-106">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4abf0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4abf0-107">Prerequisites</span></span>
<span data-ttu-id="4abf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4abf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4abf0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4abf0-110">Permission type</span></span>|<span data-ttu-id="4abf0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4abf0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4abf0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4abf0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4abf0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4abf0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4abf0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4abf0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4abf0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4abf0-115">Not supported.</span></span>|
|<span data-ttu-id="4abf0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4abf0-116">Application</span></span>|<span data-ttu-id="4abf0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4abf0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4abf0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4abf0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4abf0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4abf0-119">Optional query parameters</span></span>
<span data-ttu-id="4abf0-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4abf0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4abf0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4abf0-121">Request headers</span></span>
|<span data-ttu-id="4abf0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4abf0-122">Header</span></span>|<span data-ttu-id="4abf0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4abf0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4abf0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4abf0-124">Authorization</span></span>|<span data-ttu-id="4abf0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4abf0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4abf0-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4abf0-126">Accept</span></span>|<span data-ttu-id="4abf0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4abf0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4abf0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4abf0-128">Request body</span></span>
<span data-ttu-id="4abf0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4abf0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4abf0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4abf0-130">Response</span></span>
<span data-ttu-id="4abf0-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4abf0-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4abf0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4abf0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4abf0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4abf0-133">Request</span></span>
<span data-ttu-id="4abf0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4abf0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="4abf0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4abf0-135">Response</span></span>
<span data-ttu-id="4abf0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4abf0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1913

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
    "showOfficeWebApps": true
  }
}
```






