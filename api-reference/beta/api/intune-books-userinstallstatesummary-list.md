---
title: Listar userInstallStateSummaries
description: Listar propriedades e relações dos objetos userInstallStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d08e63e63b6d40eaa3ca99211d56e8c73799402
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760323"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="00bba-103">Listar userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="00bba-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="00bba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00bba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00bba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00bba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00bba-106">Listar propriedades e relações dos objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="00bba-106">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00bba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00bba-107">Prerequisites</span></span>
<span data-ttu-id="00bba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00bba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00bba-110">Permission type</span></span>|<span data-ttu-id="00bba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00bba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00bba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00bba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00bba-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="00bba-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="00bba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00bba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00bba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00bba-115">Not supported.</span></span>|
|<span data-ttu-id="00bba-116">Application</span><span class="sxs-lookup"><span data-stu-id="00bba-116">Application</span></span>|<span data-ttu-id="00bba-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="00bba-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00bba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00bba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="00bba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00bba-119">Request headers</span></span>
|<span data-ttu-id="00bba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00bba-120">Header</span></span>|<span data-ttu-id="00bba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="00bba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00bba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="00bba-122">Authorization</span></span>|<span data-ttu-id="00bba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00bba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00bba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00bba-124">Accept</span></span>|<span data-ttu-id="00bba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00bba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00bba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00bba-126">Request body</span></span>
<span data-ttu-id="00bba-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00bba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00bba-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="00bba-128">Response</span></span>
<span data-ttu-id="00bba-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00bba-129">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00bba-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00bba-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="00bba-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00bba-131">Request</span></span>
<span data-ttu-id="00bba-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00bba-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="00bba-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="00bba-133">Response</span></span>
<span data-ttu-id="00bba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00bba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




