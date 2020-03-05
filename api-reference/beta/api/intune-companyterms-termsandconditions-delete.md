---
title: Excluir termsAndConditions
description: Exclui termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87af4901e012dda82ff574a46e72726945b48e34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450227"
---
# <a name="delete-termsandconditions"></a><span data-ttu-id="ebb72-103">Excluir termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ebb72-103">Delete termsAndConditions</span></span>

<span data-ttu-id="ebb72-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ebb72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebb72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebb72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebb72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebb72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebb72-107">Exclui [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="ebb72-107">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebb72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebb72-108">Prerequisites</span></span>
<span data-ttu-id="ebb72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebb72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebb72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebb72-111">Permission type</span></span>|<span data-ttu-id="ebb72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebb72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebb72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebb72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebb72-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebb72-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebb72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebb72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebb72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebb72-116">Not supported.</span></span>|
|<span data-ttu-id="ebb72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebb72-117">Application</span></span>|<span data-ttu-id="ebb72-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebb72-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebb72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebb72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="ebb72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebb72-120">Request headers</span></span>
|<span data-ttu-id="ebb72-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebb72-121">Header</span></span>|<span data-ttu-id="ebb72-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebb72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebb72-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebb72-123">Authorization</span></span>|<span data-ttu-id="ebb72-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebb72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebb72-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebb72-125">Accept</span></span>|<span data-ttu-id="ebb72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebb72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebb72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebb72-127">Request body</span></span>
<span data-ttu-id="ebb72-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebb72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebb72-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebb72-129">Response</span></span>
<span data-ttu-id="ebb72-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebb72-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebb72-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebb72-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebb72-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebb72-132">Request</span></span>
<span data-ttu-id="ebb72-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebb72-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="ebb72-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebb72-134">Response</span></span>
<span data-ttu-id="ebb72-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebb72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





