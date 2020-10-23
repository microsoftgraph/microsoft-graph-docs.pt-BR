---
title: Excluir complianceManagementPartner
description: Exclui complianceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cd0b5c3c12430bf39e00f854dcc4c751f678afd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48712922"
---
# <a name="delete-compliancemanagementpartner"></a><span data-ttu-id="dc77e-103">Excluir complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="dc77e-103">Delete complianceManagementPartner</span></span>

<span data-ttu-id="dc77e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc77e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc77e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc77e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc77e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc77e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc77e-107">Exclui [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="dc77e-107">Deletes a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc77e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc77e-108">Prerequisites</span></span>
<span data-ttu-id="dc77e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc77e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc77e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc77e-111">Permission type</span></span>|<span data-ttu-id="dc77e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc77e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc77e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc77e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc77e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc77e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc77e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc77e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc77e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc77e-116">Not supported.</span></span>|
|<span data-ttu-id="dc77e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc77e-117">Application</span></span>|<span data-ttu-id="dc77e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc77e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc77e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc77e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="dc77e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc77e-120">Request headers</span></span>
|<span data-ttu-id="dc77e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc77e-121">Header</span></span>|<span data-ttu-id="dc77e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dc77e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc77e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc77e-123">Authorization</span></span>|<span data-ttu-id="dc77e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc77e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc77e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc77e-125">Accept</span></span>|<span data-ttu-id="dc77e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc77e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc77e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc77e-127">Request body</span></span>
<span data-ttu-id="dc77e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc77e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc77e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc77e-129">Response</span></span>
<span data-ttu-id="dc77e-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc77e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc77e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc77e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc77e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc77e-132">Request</span></span>
<span data-ttu-id="dc77e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc77e-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="dc77e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc77e-134">Response</span></span>
<span data-ttu-id="dc77e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc77e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





