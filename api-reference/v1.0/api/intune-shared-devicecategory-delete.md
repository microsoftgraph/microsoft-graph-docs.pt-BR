---
title: Excluir deviceCategory
description: Exclui deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 121ab846c29daf1eaf3c5b20cde8dbefc403e260
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941573"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="71212-103">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="71212-103">Delete deviceCategory</span></span>

> <span data-ttu-id="71212-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71212-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71212-105">Exclui [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="71212-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71212-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71212-106">Prerequisites</span></span>
<span data-ttu-id="71212-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71212-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71212-109">Permission type</span></span>|<span data-ttu-id="71212-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71212-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71212-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71212-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="71212-112">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="71212-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="71212-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71212-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="71212-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71212-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71212-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71212-115">Not supported.</span></span>|
|<span data-ttu-id="71212-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71212-116">Application</span></span>|<span data-ttu-id="71212-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71212-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71212-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71212-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="71212-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71212-119">Request headers</span></span>
|<span data-ttu-id="71212-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71212-120">Header</span></span>|<span data-ttu-id="71212-121">Valor</span><span class="sxs-lookup"><span data-stu-id="71212-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71212-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71212-122">Authorization</span></span>|<span data-ttu-id="71212-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71212-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71212-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71212-124">Accept</span></span>|<span data-ttu-id="71212-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71212-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71212-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71212-126">Request body</span></span>
<span data-ttu-id="71212-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71212-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71212-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="71212-128">Response</span></span>
<span data-ttu-id="71212-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="71212-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="71212-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71212-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="71212-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71212-131">Request</span></span>
<span data-ttu-id="71212-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71212-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="71212-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="71212-133">Response</span></span>
<span data-ttu-id="71212-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71212-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



