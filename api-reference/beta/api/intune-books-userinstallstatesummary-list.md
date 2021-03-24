---
title: Listar userInstallStateSummaries
description: Listar propriedades e relações dos objetos userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6821b394a1bb526c6e2a34efc07fe04b2105b37f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132951"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="9d523-103">Listar userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="9d523-103">List userInstallStateSummaries</span></span>

<span data-ttu-id="9d523-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d523-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d523-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d523-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d523-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d523-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d523-107">Listar propriedades e relações dos objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9d523-107">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d523-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d523-108">Prerequisites</span></span>
<span data-ttu-id="9d523-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d523-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d523-111">Permission type</span></span>|<span data-ttu-id="9d523-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d523-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d523-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d523-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d523-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d523-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d523-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d523-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d523-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d523-116">Not supported.</span></span>|
|<span data-ttu-id="9d523-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d523-117">Application</span></span>|<span data-ttu-id="9d523-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d523-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d523-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d523-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="9d523-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d523-120">Request headers</span></span>
|<span data-ttu-id="9d523-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d523-121">Header</span></span>|<span data-ttu-id="9d523-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9d523-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d523-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d523-123">Authorization</span></span>|<span data-ttu-id="9d523-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d523-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d523-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d523-125">Accept</span></span>|<span data-ttu-id="9d523-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d523-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d523-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d523-127">Request body</span></span>
<span data-ttu-id="9d523-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d523-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d523-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d523-129">Response</span></span>
<span data-ttu-id="9d523-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d523-130">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d523-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d523-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d523-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d523-132">Request</span></span>
<span data-ttu-id="9d523-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d523-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="9d523-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d523-134">Response</span></span>
<span data-ttu-id="9d523-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d523-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```




