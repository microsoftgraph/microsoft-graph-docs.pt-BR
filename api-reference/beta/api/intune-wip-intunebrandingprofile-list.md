---
title: Lista intuneBrandingProfiles
description: Lista as propriedades e os relacionamentos dos objetos intuneBrandingProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4da0a5c1109ade245a8cc2f22bb55fd1c4b49504
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944695"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="c5189-103">Lista intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="c5189-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="c5189-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c5189-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5189-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c5189-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5189-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5189-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5189-107">Lista as propriedades e os relacionamentos dos objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c5189-107">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5189-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5189-108">Prerequisites</span></span>
<span data-ttu-id="c5189-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5189-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5189-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5189-111">Permission type</span></span>|<span data-ttu-id="c5189-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5189-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5189-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5189-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5189-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5189-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c5189-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5189-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5189-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5189-116">Not supported.</span></span>|
|<span data-ttu-id="c5189-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5189-117">Application</span></span>|<span data-ttu-id="c5189-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5189-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5189-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5189-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c5189-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5189-120">Request headers</span></span>
|<span data-ttu-id="c5189-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5189-121">Header</span></span>|<span data-ttu-id="c5189-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c5189-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5189-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5189-123">Authorization</span></span>|<span data-ttu-id="c5189-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5189-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5189-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5189-125">Accept</span></span>|<span data-ttu-id="c5189-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5189-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5189-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5189-127">Request body</span></span>
<span data-ttu-id="c5189-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5189-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5189-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5189-129">Response</span></span>
<span data-ttu-id="c5189-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5189-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5189-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5189-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5189-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5189-132">Request</span></span>
<span data-ttu-id="c5189-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5189-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="c5189-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5189-134">Response</span></span>
<span data-ttu-id="c5189-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5189-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





