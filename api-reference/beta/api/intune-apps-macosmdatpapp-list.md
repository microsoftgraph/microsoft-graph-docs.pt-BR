---
title: Listar macOSMdatpApps
description: Listar Propriedades e relações dos objetos macOSMdatpApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0aae98d406f50c65c2a7f311d94e945feda16fd
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160835"
---
# <a name="list-macosmdatpapps"></a><span data-ttu-id="74ecf-103">Listar macOSMdatpApps</span><span class="sxs-lookup"><span data-stu-id="74ecf-103">List macOSMdatpApps</span></span>

> <span data-ttu-id="74ecf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74ecf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74ecf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74ecf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74ecf-106">Listar Propriedades e relações dos objetos [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="74ecf-106">List properties and relationships of the [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74ecf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74ecf-107">Prerequisites</span></span>
<span data-ttu-id="74ecf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ecf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74ecf-110">Permission type</span></span>|<span data-ttu-id="74ecf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74ecf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74ecf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74ecf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74ecf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="74ecf-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="74ecf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74ecf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74ecf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74ecf-115">Not supported.</span></span>|
|<span data-ttu-id="74ecf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74ecf-116">Application</span></span>|<span data-ttu-id="74ecf-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="74ecf-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74ecf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74ecf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="74ecf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74ecf-119">Request headers</span></span>
|<span data-ttu-id="74ecf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74ecf-120">Header</span></span>|<span data-ttu-id="74ecf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="74ecf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74ecf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="74ecf-122">Authorization</span></span>|<span data-ttu-id="74ecf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74ecf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74ecf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74ecf-124">Accept</span></span>|<span data-ttu-id="74ecf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74ecf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74ecf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74ecf-126">Request body</span></span>
<span data-ttu-id="74ecf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74ecf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74ecf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="74ecf-128">Response</span></span>
<span data-ttu-id="74ecf-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74ecf-129">If successful, this method returns a `200 OK` response code and a collection of [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ecf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74ecf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="74ecf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74ecf-131">Request</span></span>
<span data-ttu-id="74ecf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74ecf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="74ecf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="74ecf-133">Response</span></span>
<span data-ttu-id="74ecf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74ecf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1017

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSMdatpApp",
      "id": "2963b007-b007-2963-07b0-632907b06329",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "dependentAppCount": 1
    }
  ]
}
```





