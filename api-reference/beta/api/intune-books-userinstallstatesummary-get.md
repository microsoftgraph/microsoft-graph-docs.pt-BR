---
title: Get userInstallStateSummary
description: Ler propriedades e relações do objeto userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13be6bcd207d1e0cc329780217f54c10b4633fd4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132965"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="3ee34-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="3ee34-103">Get userInstallStateSummary</span></span>

<span data-ttu-id="3ee34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ee34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ee34-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ee34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ee34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ee34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ee34-107">Ler propriedades e relações do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3ee34-107">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ee34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ee34-108">Prerequisites</span></span>
<span data-ttu-id="3ee34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ee34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ee34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ee34-111">Permission type</span></span>|<span data-ttu-id="3ee34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ee34-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ee34-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ee34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ee34-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ee34-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ee34-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ee34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ee34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ee34-116">Not supported.</span></span>|
|<span data-ttu-id="3ee34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ee34-117">Application</span></span>|<span data-ttu-id="3ee34-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ee34-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ee34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ee34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ee34-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ee34-120">Optional query parameters</span></span>
<span data-ttu-id="3ee34-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee34-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ee34-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee34-122">Request headers</span></span>
|<span data-ttu-id="3ee34-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ee34-123">Header</span></span>|<span data-ttu-id="3ee34-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3ee34-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ee34-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ee34-125">Authorization</span></span>|<span data-ttu-id="3ee34-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ee34-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ee34-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ee34-127">Accept</span></span>|<span data-ttu-id="3ee34-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3ee34-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ee34-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee34-129">Request body</span></span>
<span data-ttu-id="3ee34-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ee34-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee34-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee34-131">Response</span></span>
<span data-ttu-id="3ee34-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee34-132">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ee34-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ee34-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ee34-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee34-134">Request</span></span>
<span data-ttu-id="3ee34-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ee34-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="3ee34-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee34-136">Response</span></span>
<span data-ttu-id="3ee34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ee34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```




