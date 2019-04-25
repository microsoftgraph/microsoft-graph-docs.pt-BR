---
title: Listar Navegaçãointunebrandingprofiles
description: Listar Propriedades e relações dos objetos intuneBrandingProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ab4815c69d9ce38a127e58e96cd269a87635aff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541861"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="daa47-103">Listar Navegaçãointunebrandingprofiles</span><span class="sxs-lookup"><span data-stu-id="daa47-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="daa47-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="daa47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daa47-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="daa47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daa47-106">Listar Propriedades e relações dos objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="daa47-106">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daa47-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="daa47-107">Prerequisites</span></span>
<span data-ttu-id="daa47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daa47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daa47-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daa47-110">Permission type</span></span>|<span data-ttu-id="daa47-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="daa47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daa47-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daa47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="daa47-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa47-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="daa47-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daa47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daa47-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daa47-115">Not supported.</span></span>|
|<span data-ttu-id="daa47-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daa47-116">Application</span></span>|<span data-ttu-id="daa47-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daa47-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="daa47-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daa47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="daa47-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daa47-119">Request headers</span></span>
|<span data-ttu-id="daa47-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="daa47-120">Header</span></span>|<span data-ttu-id="daa47-121">Valor</span><span class="sxs-lookup"><span data-stu-id="daa47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daa47-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="daa47-122">Authorization</span></span>|<span data-ttu-id="daa47-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daa47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daa47-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="daa47-124">Accept</span></span>|<span data-ttu-id="daa47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="daa47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daa47-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daa47-126">Request body</span></span>
<span data-ttu-id="daa47-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="daa47-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daa47-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="daa47-128">Response</span></span>
<span data-ttu-id="daa47-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daa47-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daa47-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="daa47-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="daa47-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daa47-131">Request</span></span>
<span data-ttu-id="daa47-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="daa47-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="daa47-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="daa47-133">Response</span></span>
<span data-ttu-id="daa47-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daa47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1562

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
  ]
}
```





