---
title: Excluir deviceCategory
description: Exclui deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd38e1eb6f732db629a6c88a9a4a36e0357431df
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732249"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="bbfc8-103">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bbfc8-103">Delete deviceCategory</span></span>

<span data-ttu-id="bbfc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbfc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbfc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbfc8-106">Exclui [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="bbfc8-106">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbfc8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbfc8-107">Prerequisites</span></span>
<span data-ttu-id="bbfc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbfc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbfc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbfc8-110">Permission type</span></span>|<span data-ttu-id="bbfc8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bbfc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbfc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbfc8-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bbfc8-113">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="bbfc8-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="bbfc8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbfc8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bbfc8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbfc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbfc8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-116">Not supported.</span></span>|
|<span data-ttu-id="bbfc8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbfc8-117">Application</span></span>|<span data-ttu-id="bbfc8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbfc8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbfc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="bbfc8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfc8-120">Request headers</span></span>
|<span data-ttu-id="bbfc8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbfc8-121">Header</span></span>|<span data-ttu-id="bbfc8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bbfc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbfc8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbfc8-123">Authorization</span></span>|<span data-ttu-id="bbfc8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbfc8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbfc8-125">Accept</span></span>|<span data-ttu-id="bbfc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbfc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbfc8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfc8-127">Request body</span></span>
<span data-ttu-id="bbfc8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbfc8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbfc8-129">Response</span></span>
<span data-ttu-id="bbfc8-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bbfc8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbfc8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbfc8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfc8-132">Request</span></span>
<span data-ttu-id="bbfc8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="bbfc8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbfc8-134">Response</span></span>
<span data-ttu-id="bbfc8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbfc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









