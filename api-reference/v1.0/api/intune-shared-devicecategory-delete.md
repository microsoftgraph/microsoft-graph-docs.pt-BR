---
title: Excluir deviceCategory
description: Exclui deviceCategory.
author: tfitzmac
ms.openlocfilehash: 04c5d2f0c062e2cd5b5c066415e26273ef4d9231
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331644"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="5b5dd-103">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5b5dd-103">Delete deviceCategory</span></span>

> <span data-ttu-id="5b5dd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b5dd-105">Exclui [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5b5dd-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b5dd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b5dd-106">Prerequisites</span></span>
<span data-ttu-id="5b5dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b5dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b5dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b5dd-109">Permission type</span></span>|<span data-ttu-id="5b5dd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b5dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b5dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b5dd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5b5dd-112">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="5b5dd-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5b5dd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b5dd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5b5dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b5dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b5dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-115">Not supported.</span></span>|
|<span data-ttu-id="5b5dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b5dd-116">Application</span></span>|<span data-ttu-id="5b5dd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b5dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b5dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5b5dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b5dd-119">Request headers</span></span>
|<span data-ttu-id="5b5dd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b5dd-120">Header</span></span>|<span data-ttu-id="5b5dd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b5dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b5dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b5dd-122">Authorization</span></span>|<span data-ttu-id="5b5dd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b5dd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b5dd-124">Accept</span></span>|<span data-ttu-id="5b5dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b5dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b5dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b5dd-126">Request body</span></span>
<span data-ttu-id="5b5dd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b5dd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b5dd-128">Response</span></span>
<span data-ttu-id="5b5dd-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b5dd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b5dd-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b5dd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b5dd-131">Request</span></span>
<span data-ttu-id="5b5dd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="5b5dd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b5dd-133">Response</span></span>
<span data-ttu-id="5b5dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



