---
title: Excluir mdmWindowsInformationProtectionPolicy
description: Exclui mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b1e03393901a2b50a99e05d698856032315021f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458354"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="79efc-103">Excluir mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="79efc-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="79efc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="79efc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79efc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79efc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79efc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79efc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79efc-107">Exclui [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="79efc-107">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79efc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79efc-108">Prerequisites</span></span>
<span data-ttu-id="79efc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79efc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79efc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79efc-111">Permission type</span></span>|<span data-ttu-id="79efc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79efc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79efc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79efc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="79efc-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="79efc-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="79efc-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79efc-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="79efc-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="79efc-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="79efc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79efc-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79efc-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79efc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79efc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79efc-119">Not supported.</span></span>|
|<span data-ttu-id="79efc-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79efc-120">Application</span></span>||
| <span data-ttu-id="79efc-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="79efc-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="79efc-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79efc-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="79efc-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="79efc-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="79efc-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79efc-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79efc-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79efc-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="79efc-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79efc-126">Request headers</span></span>
|<span data-ttu-id="79efc-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79efc-127">Header</span></span>|<span data-ttu-id="79efc-128">Valor</span><span class="sxs-lookup"><span data-stu-id="79efc-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79efc-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="79efc-129">Authorization</span></span>|<span data-ttu-id="79efc-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79efc-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79efc-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79efc-131">Accept</span></span>|<span data-ttu-id="79efc-132">application/json</span><span class="sxs-lookup"><span data-stu-id="79efc-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79efc-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79efc-133">Request body</span></span>
<span data-ttu-id="79efc-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79efc-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79efc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="79efc-135">Response</span></span>
<span data-ttu-id="79efc-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79efc-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79efc-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79efc-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="79efc-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79efc-138">Request</span></span>
<span data-ttu-id="79efc-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79efc-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="79efc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="79efc-140">Response</span></span>
<span data-ttu-id="79efc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79efc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








