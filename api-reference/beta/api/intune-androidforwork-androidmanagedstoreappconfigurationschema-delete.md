---
title: Excluir androidManagedStoreAppConfigurationSchema
description: Exclui androidManagedStoreAppConfigurationSchema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 684ca836cd2815d4ddfbc7f5b07fad028dfd0ec2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980562"
---
# <a name="delete-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="10e18-103">Excluir androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="10e18-103">Delete androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="10e18-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10e18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10e18-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10e18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10e18-106">Exclui [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="10e18-106">Deletes a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10e18-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10e18-107">Prerequisites</span></span>
<span data-ttu-id="10e18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10e18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10e18-110">Permission type</span></span>|<span data-ttu-id="10e18-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10e18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10e18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10e18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10e18-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10e18-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10e18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10e18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10e18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10e18-115">Not supported.</span></span>|
|<span data-ttu-id="10e18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10e18-116">Application</span></span>|<span data-ttu-id="10e18-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10e18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10e18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10e18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="10e18-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10e18-119">Request headers</span></span>
|<span data-ttu-id="10e18-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10e18-120">Header</span></span>|<span data-ttu-id="10e18-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10e18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10e18-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10e18-122">Authorization</span></span>|<span data-ttu-id="10e18-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10e18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10e18-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10e18-124">Accept</span></span>|<span data-ttu-id="10e18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10e18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e18-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10e18-126">Request body</span></span>
<span data-ttu-id="10e18-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10e18-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10e18-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="10e18-128">Response</span></span>
<span data-ttu-id="10e18-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="10e18-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="10e18-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10e18-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="10e18-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10e18-131">Request</span></span>
<span data-ttu-id="10e18-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10e18-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="10e18-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="10e18-133">Response</span></span>
<span data-ttu-id="10e18-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10e18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




