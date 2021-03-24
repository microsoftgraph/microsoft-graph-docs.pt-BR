---
title: Listar managedApps
description: Listar propriedades e relações dos objetos managedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c96118476d082f7d6ad2c6ca71f8b20b49d2ebe4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140242"
---
# <a name="list-managedapps"></a><span data-ttu-id="67178-103">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="67178-103">List managedApps</span></span>

<span data-ttu-id="67178-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67178-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67178-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67178-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67178-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67178-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67178-107">Listar propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="67178-107">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67178-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67178-108">Prerequisites</span></span>
<span data-ttu-id="67178-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67178-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67178-111">Permission type</span></span>|<span data-ttu-id="67178-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67178-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67178-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67178-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67178-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67178-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67178-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67178-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67178-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67178-116">Not supported.</span></span>|
|<span data-ttu-id="67178-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67178-117">Application</span></span>|<span data-ttu-id="67178-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67178-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67178-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67178-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="67178-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67178-120">Request headers</span></span>
|<span data-ttu-id="67178-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67178-121">Header</span></span>|<span data-ttu-id="67178-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67178-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67178-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67178-123">Authorization</span></span>|<span data-ttu-id="67178-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67178-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67178-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67178-125">Accept</span></span>|<span data-ttu-id="67178-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67178-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67178-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67178-127">Request body</span></span>
<span data-ttu-id="67178-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67178-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67178-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67178-129">Response</span></span>
<span data-ttu-id="67178-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedApp](../resources/intune-apps-managedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67178-130">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67178-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67178-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="67178-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67178-132">Request</span></span>
<span data-ttu-id="67178-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67178-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="67178-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="67178-134">Response</span></span>
<span data-ttu-id="67178-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67178-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1158

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedApp",
      "id": "f687dd85-dd85-f687-85dd-87f685dd87f6",
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
      "dependentAppCount": 1,
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
      "appAvailability": "lineOfBusiness",
      "version": "Version value"
    }
  ]
}
```




