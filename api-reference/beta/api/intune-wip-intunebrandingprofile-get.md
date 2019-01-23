---
title: Obter intuneBrandingProfile
description: Leia as propriedades e os relacionamentos do objeto intuneBrandingProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5efcfcabcb84dae77e91d7d3c765b18c9d95783c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402997"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="7d25f-103">Obter intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="7d25f-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="7d25f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d25f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d25f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d25f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d25f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7d25f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d25f-107">Leia as propriedades e os relacionamentos do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7d25f-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d25f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d25f-108">Prerequisites</span></span>
<span data-ttu-id="7d25f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d25f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7d25f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d25f-111">Permission type</span></span>|<span data-ttu-id="7d25f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d25f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d25f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d25f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d25f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d25f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7d25f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d25f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d25f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d25f-116">Not supported.</span></span>|
|<span data-ttu-id="7d25f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d25f-117">Application</span></span>|<span data-ttu-id="7d25f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d25f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d25f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d25f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d25f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d25f-120">Optional query parameters</span></span>
<span data-ttu-id="7d25f-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d25f-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d25f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d25f-122">Request headers</span></span>
|<span data-ttu-id="7d25f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d25f-123">Header</span></span>|<span data-ttu-id="7d25f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7d25f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d25f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d25f-125">Authorization</span></span>|<span data-ttu-id="7d25f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d25f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d25f-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d25f-127">Accept</span></span>|<span data-ttu-id="7d25f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d25f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d25f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d25f-129">Request body</span></span>
<span data-ttu-id="7d25f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d25f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d25f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d25f-131">Response</span></span>
<span data-ttu-id="7d25f-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d25f-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d25f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d25f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d25f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d25f-134">Request</span></span>
<span data-ttu-id="7d25f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d25f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="7d25f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d25f-136">Response</span></span>
<span data-ttu-id="7d25f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d25f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




