---
title: Obter intuneBrandingProfile
description: Leia as propriedades e as relações do objeto intuneBrandingProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a17a41f5fe803f1ceb579b3207d34cd8f85e91b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798779"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="e1fdc-103">Obter intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="e1fdc-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="e1fdc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1fdc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1fdc-106">Leia as propriedades e as relações do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e1fdc-106">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1fdc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1fdc-107">Prerequisites</span></span>
<span data-ttu-id="e1fdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1fdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1fdc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1fdc-110">Permission type</span></span>|<span data-ttu-id="e1fdc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1fdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1fdc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1fdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1fdc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1fdc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1fdc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1fdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1fdc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-115">Not supported.</span></span>|
|<span data-ttu-id="e1fdc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1fdc-116">Application</span></span>|<span data-ttu-id="e1fdc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1fdc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1fdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1fdc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1fdc-119">Optional query parameters</span></span>
<span data-ttu-id="e1fdc-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1fdc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fdc-121">Request headers</span></span>
|<span data-ttu-id="e1fdc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1fdc-122">Header</span></span>|<span data-ttu-id="e1fdc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e1fdc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1fdc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1fdc-124">Authorization</span></span>|<span data-ttu-id="e1fdc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1fdc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1fdc-126">Accept</span></span>|<span data-ttu-id="e1fdc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e1fdc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1fdc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fdc-128">Request body</span></span>
<span data-ttu-id="e1fdc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1fdc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fdc-130">Response</span></span>
<span data-ttu-id="e1fdc-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1fdc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1fdc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1fdc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fdc-133">Request</span></span>
<span data-ttu-id="e1fdc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="e1fdc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fdc-135">Response</span></span>
<span data-ttu-id="e1fdc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1fdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1472

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
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
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
    }
  }
}
```





