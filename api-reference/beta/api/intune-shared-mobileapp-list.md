---
title: Listar mobileApps
description: Listar propriedades e relações dos objetos mobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29452b73b3ccd2de94b30b3cdc7dc4118292027c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694295"
---
# <a name="list-mobileapps"></a><span data-ttu-id="88e50-103">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="88e50-103">List mobileApps</span></span>

<span data-ttu-id="88e50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88e50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88e50-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88e50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88e50-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88e50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88e50-107">Listar propriedades e relações dos objetos [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="88e50-107">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88e50-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88e50-108">Prerequisites</span></span>
<span data-ttu-id="88e50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88e50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e50-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88e50-111">Permission type</span></span>|<span data-ttu-id="88e50-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88e50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88e50-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88e50-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88e50-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="88e50-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="88e50-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e50-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="88e50-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="88e50-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88e50-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e50-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="88e50-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88e50-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88e50-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88e50-119">Not supported.</span></span>|
|<span data-ttu-id="88e50-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88e50-120">Application</span></span>||
| <span data-ttu-id="88e50-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="88e50-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="88e50-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e50-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="88e50-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="88e50-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88e50-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e50-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88e50-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88e50-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="88e50-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88e50-126">Request headers</span></span>
|<span data-ttu-id="88e50-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88e50-127">Header</span></span>|<span data-ttu-id="88e50-128">Valor</span><span class="sxs-lookup"><span data-stu-id="88e50-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88e50-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="88e50-129">Authorization</span></span>|<span data-ttu-id="88e50-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88e50-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88e50-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88e50-131">Accept</span></span>|<span data-ttu-id="88e50-132">application/json</span><span class="sxs-lookup"><span data-stu-id="88e50-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88e50-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88e50-133">Request body</span></span>
<span data-ttu-id="88e50-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88e50-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88e50-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="88e50-135">Response</span></span>
<span data-ttu-id="88e50-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileApp](../resources/intune-shared-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88e50-136">If successful, this method returns a `200 OK` response code and a collection of [mobileApp](../resources/intune-shared-mobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88e50-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88e50-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="88e50-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88e50-138">Request</span></span>
<span data-ttu-id="88e50-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88e50-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="88e50-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="88e50-140">Response</span></span>
<span data-ttu-id="88e50-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88e50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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








