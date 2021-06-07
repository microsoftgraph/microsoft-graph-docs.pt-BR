---
title: Excluir resourceOperation
description: Exclui resourceOperation
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6be3d24fdb1e12f76dae3053c0b830b20fc2648d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751444"
---
# <a name="delete-resourceoperation"></a><span data-ttu-id="6968e-103">Excluir resourceOperation</span><span class="sxs-lookup"><span data-stu-id="6968e-103">Delete resourceOperation</span></span>

<span data-ttu-id="6968e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6968e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6968e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6968e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6968e-106">Exclui [resourceOperation](../resources/intune-rbac-resourceoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6968e-106">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6968e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6968e-107">Prerequisites</span></span>
<span data-ttu-id="6968e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6968e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6968e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6968e-110">Permission type</span></span>|<span data-ttu-id="6968e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6968e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6968e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6968e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6968e-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6968e-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6968e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6968e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6968e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6968e-115">Not supported.</span></span>|
|<span data-ttu-id="6968e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6968e-116">Application</span></span>|<span data-ttu-id="6968e-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6968e-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6968e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6968e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="6968e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6968e-119">Request headers</span></span>
|<span data-ttu-id="6968e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6968e-120">Header</span></span>|<span data-ttu-id="6968e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6968e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6968e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6968e-122">Authorization</span></span>|<span data-ttu-id="6968e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6968e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6968e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6968e-124">Accept</span></span>|<span data-ttu-id="6968e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6968e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6968e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6968e-126">Request body</span></span>
<span data-ttu-id="6968e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6968e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6968e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6968e-128">Response</span></span>
<span data-ttu-id="6968e-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6968e-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6968e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6968e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6968e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6968e-131">Request</span></span>
<span data-ttu-id="6968e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6968e-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="6968e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6968e-133">Response</span></span>
<span data-ttu-id="6968e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6968e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




