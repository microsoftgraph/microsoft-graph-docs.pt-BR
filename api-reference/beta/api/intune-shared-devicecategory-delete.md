---
title: Excluir deviceCategory
description: Exclui deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1939a4e5a1598d0714309e58891f544ae43f34b9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940156"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="f47bb-103">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f47bb-103">Delete deviceCategory</span></span>

> <span data-ttu-id="f47bb-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f47bb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f47bb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f47bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f47bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f47bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f47bb-107">Exclui [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="f47bb-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f47bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f47bb-108">Prerequisites</span></span>
<span data-ttu-id="f47bb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f47bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f47bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f47bb-111">Permission type</span></span>|<span data-ttu-id="f47bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f47bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f47bb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f47bb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f47bb-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="f47bb-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f47bb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f47bb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f47bb-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f47bb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f47bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f47bb-117">Not supported.</span></span>|
|<span data-ttu-id="f47bb-118">Application</span><span class="sxs-lookup"><span data-stu-id="f47bb-118">Application</span></span>||
| <span data-ttu-id="f47bb-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="f47bb-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f47bb-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f47bb-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f47bb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f47bb-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f47bb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f47bb-122">Request headers</span></span>
|<span data-ttu-id="f47bb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f47bb-123">Header</span></span>|<span data-ttu-id="f47bb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f47bb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f47bb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f47bb-125">Authorization</span></span>|<span data-ttu-id="f47bb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f47bb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f47bb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f47bb-127">Accept</span></span>|<span data-ttu-id="f47bb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f47bb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f47bb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f47bb-129">Request body</span></span>
<span data-ttu-id="f47bb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f47bb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f47bb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f47bb-131">Response</span></span>
<span data-ttu-id="f47bb-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f47bb-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f47bb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f47bb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f47bb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f47bb-134">Request</span></span>

<span data-ttu-id="f47bb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f47bb-135">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="f47bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f47bb-136">Response</span></span>

<span data-ttu-id="f47bb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f47bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```











