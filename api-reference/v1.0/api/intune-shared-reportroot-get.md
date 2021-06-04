---
title: Get reportRoot
description: Ler propriedades e relações do objeto reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d22989835a5311a1ee7f09618becc38a389975b
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732213"
---
# <a name="get-reportroot"></a><span data-ttu-id="d9b43-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="d9b43-103">Get reportRoot</span></span>

<span data-ttu-id="d9b43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9b43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9b43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9b43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9b43-106">Ler propriedades e relações do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d9b43-106">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9b43-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9b43-107">Prerequisites</span></span>
<span data-ttu-id="d9b43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9b43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9b43-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9b43-110">Permission type</span></span>|<span data-ttu-id="d9b43-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9b43-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9b43-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9b43-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d9b43-113">&nbsp;&nbsp;Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d9b43-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="d9b43-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9b43-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d9b43-115">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="d9b43-115">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="d9b43-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9b43-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d9b43-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9b43-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9b43-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9b43-118">Not supported.</span></span>|
|<span data-ttu-id="d9b43-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9b43-119">Application</span></span>|<span data-ttu-id="d9b43-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9b43-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9b43-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9b43-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9b43-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9b43-122">Optional query parameters</span></span>
<span data-ttu-id="d9b43-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9b43-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d9b43-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b43-124">Request headers</span></span>
|<span data-ttu-id="d9b43-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9b43-125">Header</span></span>|<span data-ttu-id="d9b43-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d9b43-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9b43-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9b43-127">Authorization</span></span>|<span data-ttu-id="d9b43-128">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9b43-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9b43-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9b43-129">Accept</span></span>|<span data-ttu-id="d9b43-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d9b43-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b43-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b43-131">Request body</span></span>
<span data-ttu-id="d9b43-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9b43-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9b43-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9b43-133">Response</span></span>
<span data-ttu-id="d9b43-134">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9b43-134">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9b43-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9b43-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9b43-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b43-136">Request</span></span>
<span data-ttu-id="d9b43-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9b43-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="d9b43-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9b43-138">Response</span></span>
<span data-ttu-id="d9b43-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9b43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```