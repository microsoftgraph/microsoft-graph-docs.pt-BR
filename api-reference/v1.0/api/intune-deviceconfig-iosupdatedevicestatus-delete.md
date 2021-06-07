---
title: Excluir iosUpdateDeviceStatus
description: Exclui iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 223ec5a8d6890c95e10b8ebc8dc7f6504858ba02
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756306"
---
# <a name="delete-iosupdatedevicestatus"></a><span data-ttu-id="75ff3-103">Excluir iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="75ff3-103">Delete iosUpdateDeviceStatus</span></span>

<span data-ttu-id="75ff3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75ff3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75ff3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75ff3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75ff3-106">Exclui [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-106">Deletes a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75ff3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75ff3-107">Prerequisites</span></span>
<span data-ttu-id="75ff3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75ff3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75ff3-110">Permission type</span></span>|<span data-ttu-id="75ff3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75ff3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75ff3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75ff3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75ff3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75ff3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75ff3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75ff3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75ff3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75ff3-115">Not supported.</span></span>|
|<span data-ttu-id="75ff3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75ff3-116">Application</span></span>|<span data-ttu-id="75ff3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75ff3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75ff3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75ff3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="75ff3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75ff3-119">Request headers</span></span>
|<span data-ttu-id="75ff3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75ff3-120">Header</span></span>|<span data-ttu-id="75ff3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="75ff3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75ff3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="75ff3-122">Authorization</span></span>|<span data-ttu-id="75ff3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75ff3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75ff3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75ff3-124">Accept</span></span>|<span data-ttu-id="75ff3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75ff3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75ff3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75ff3-126">Request body</span></span>
<span data-ttu-id="75ff3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75ff3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75ff3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="75ff3-128">Response</span></span>
<span data-ttu-id="75ff3-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75ff3-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75ff3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75ff3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="75ff3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75ff3-131">Request</span></span>
<span data-ttu-id="75ff3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75ff3-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="75ff3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="75ff3-133">Response</span></span>
<span data-ttu-id="75ff3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75ff3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




