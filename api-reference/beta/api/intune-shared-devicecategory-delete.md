---
title: Excluir deviceCategory
description: Exclui deviceCategory.
author: tfitzmac
ms.openlocfilehash: ea8f8860f79cc0c14e985c64a1457b114d30b6b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321291"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="e4571-103">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="e4571-103">Delete deviceCategory</span></span>

> <span data-ttu-id="e4571-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4571-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4571-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4571-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4571-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e4571-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4571-107">Exclui [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="e4571-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4571-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4571-108">Prerequisites</span></span>
<span data-ttu-id="e4571-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4571-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4571-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4571-111">Permission type</span></span>|<span data-ttu-id="e4571-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4571-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4571-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4571-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e4571-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="e4571-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e4571-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4571-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e4571-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4571-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4571-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4571-117">Not supported.</span></span>|
|<span data-ttu-id="e4571-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4571-118">Application</span></span>|<span data-ttu-id="e4571-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4571-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4571-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4571-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="e4571-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4571-121">Request headers</span></span>
|<span data-ttu-id="e4571-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4571-122">Header</span></span>|<span data-ttu-id="e4571-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e4571-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4571-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4571-124">Authorization</span></span>|<span data-ttu-id="e4571-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4571-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4571-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e4571-126">Accept</span></span>|<span data-ttu-id="e4571-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e4571-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4571-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4571-128">Request body</span></span>
<span data-ttu-id="e4571-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4571-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4571-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4571-130">Response</span></span>
<span data-ttu-id="e4571-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4571-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4571-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4571-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4571-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4571-133">Request</span></span>

<span data-ttu-id="e4571-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4571-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="e4571-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4571-135">Response</span></span>

<span data-ttu-id="e4571-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4571-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



