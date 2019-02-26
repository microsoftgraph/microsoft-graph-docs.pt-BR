---
title: Excluir deviceCategory
description: Exclui deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35dffc1c280caeb10007dbf11d390ac7487d4a61
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249967"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="78dde-103">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="78dde-103">Delete deviceCategory</span></span>

> <span data-ttu-id="78dde-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78dde-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78dde-105">Exclui [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="78dde-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78dde-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78dde-106">Prerequisites</span></span>
<span data-ttu-id="78dde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78dde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78dde-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78dde-109">Permission type</span></span>|<span data-ttu-id="78dde-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78dde-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78dde-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78dde-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="78dde-112">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="78dde-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="78dde-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78dde-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78dde-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78dde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78dde-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78dde-115">Not supported.</span></span>|
|<span data-ttu-id="78dde-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78dde-116">Application</span></span>|<span data-ttu-id="78dde-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78dde-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78dde-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78dde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="78dde-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78dde-119">Request headers</span></span>
|<span data-ttu-id="78dde-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78dde-120">Header</span></span>|<span data-ttu-id="78dde-121">Valor</span><span class="sxs-lookup"><span data-stu-id="78dde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78dde-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78dde-122">Authorization</span></span>|<span data-ttu-id="78dde-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78dde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78dde-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78dde-124">Accept</span></span>|<span data-ttu-id="78dde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78dde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78dde-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78dde-126">Request body</span></span>
<span data-ttu-id="78dde-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78dde-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78dde-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="78dde-128">Response</span></span>
<span data-ttu-id="78dde-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="78dde-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="78dde-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78dde-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="78dde-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78dde-131">Request</span></span>
<span data-ttu-id="78dde-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78dde-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="78dde-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78dde-133">Response</span></span>
<span data-ttu-id="78dde-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78dde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



