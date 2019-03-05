---
title: Excluir roleDefinition
description: Exclui roleDefinition
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f9731b6ee993664f9b6d9a66c78dcaa015b10d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158818"
---
# <a name="delete-roledefinition"></a><span data-ttu-id="a7817-103">Excluir roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a7817-103">Delete roleDefinition</span></span>

> <span data-ttu-id="a7817-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7817-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7817-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7817-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7817-106">Exclui [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a7817-106">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7817-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7817-107">Prerequisites</span></span>
<span data-ttu-id="a7817-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7817-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7817-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7817-110">Permission type</span></span>|<span data-ttu-id="a7817-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7817-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7817-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7817-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7817-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7817-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a7817-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7817-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7817-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7817-115">Not supported.</span></span>|
|<span data-ttu-id="a7817-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7817-116">Application</span></span>|<span data-ttu-id="a7817-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7817-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7817-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7817-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="a7817-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7817-119">Request headers</span></span>
|<span data-ttu-id="a7817-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7817-120">Header</span></span>|<span data-ttu-id="a7817-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a7817-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7817-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7817-122">Authorization</span></span>|<span data-ttu-id="a7817-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7817-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7817-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7817-124">Accept</span></span>|<span data-ttu-id="a7817-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7817-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7817-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7817-126">Request body</span></span>
<span data-ttu-id="a7817-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7817-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7817-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7817-128">Response</span></span>
<span data-ttu-id="a7817-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7817-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7817-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7817-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7817-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7817-131">Request</span></span>
<span data-ttu-id="a7817-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7817-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="a7817-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7817-133">Response</span></span>
<span data-ttu-id="a7817-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7817-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




