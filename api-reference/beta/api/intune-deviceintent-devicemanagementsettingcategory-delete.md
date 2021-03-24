---
title: Excluir deviceManagementSettingCategory
description: Exclui um deviceManagementSettingCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69f7d03926759fd90f24c16ea108482e4f8ca8eb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136675"
---
# <a name="delete-devicemanagementsettingcategory"></a><span data-ttu-id="6ad79-103">Excluir deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="6ad79-103">Delete deviceManagementSettingCategory</span></span>

<span data-ttu-id="6ad79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ad79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ad79-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ad79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ad79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ad79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ad79-107">Exclui um [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span><span class="sxs-lookup"><span data-stu-id="6ad79-107">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ad79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ad79-108">Prerequisites</span></span>
<span data-ttu-id="6ad79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ad79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ad79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ad79-111">Permission type</span></span>|<span data-ttu-id="6ad79-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ad79-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ad79-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ad79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ad79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ad79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ad79-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ad79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ad79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ad79-116">Not supported.</span></span>|
|<span data-ttu-id="6ad79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ad79-117">Application</span></span>|<span data-ttu-id="6ad79-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ad79-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ad79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ad79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="6ad79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad79-120">Request headers</span></span>
|<span data-ttu-id="6ad79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ad79-121">Header</span></span>|<span data-ttu-id="6ad79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ad79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ad79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ad79-123">Authorization</span></span>|<span data-ttu-id="6ad79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ad79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ad79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ad79-125">Accept</span></span>|<span data-ttu-id="6ad79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ad79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ad79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad79-127">Request body</span></span>
<span data-ttu-id="6ad79-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ad79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ad79-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ad79-129">Response</span></span>
<span data-ttu-id="6ad79-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6ad79-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6ad79-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ad79-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ad79-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad79-132">Request</span></span>
<span data-ttu-id="6ad79-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ad79-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
```

### <a name="response"></a><span data-ttu-id="6ad79-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ad79-134">Response</span></span>
<span data-ttu-id="6ad79-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ad79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




