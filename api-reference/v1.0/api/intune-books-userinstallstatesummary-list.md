---
title: Listar userInstallStateSummaries
description: Listar propriedades e relações dos objetos userInstallStateSummary.
ms.openlocfilehash: 9c28b1b8ab7fd4b3d9b009bc4e436c8de9f64c54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007142"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="b4266-103">Listar userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="b4266-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="b4266-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4266-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4266-105">Listar propriedades e relações dos objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b4266-105">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4266-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4266-106">Prerequisites</span></span>
<span data-ttu-id="b4266-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4266-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4266-109">Permission type</span></span>|<span data-ttu-id="b4266-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4266-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4266-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4266-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4266-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4266-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b4266-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4266-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4266-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4266-114">Not supported.</span></span>|
|<span data-ttu-id="b4266-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4266-115">Application</span></span>|<span data-ttu-id="b4266-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4266-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4266-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4266-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="b4266-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4266-118">Request headers</span></span>
|<span data-ttu-id="b4266-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4266-119">Header</span></span>|<span data-ttu-id="b4266-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b4266-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4266-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4266-121">Authorization</span></span>|<span data-ttu-id="b4266-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4266-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4266-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b4266-123">Accept</span></span>|<span data-ttu-id="b4266-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4266-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4266-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4266-125">Request body</span></span>
<span data-ttu-id="b4266-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4266-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4266-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4266-127">Response</span></span>
<span data-ttu-id="b4266-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4266-128">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4266-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4266-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4266-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4266-130">Request</span></span>
<span data-ttu-id="b4266-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4266-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="b4266-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4266-132">Response</span></span>
<span data-ttu-id="b4266-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4266-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



