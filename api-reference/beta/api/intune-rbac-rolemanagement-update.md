---
title: Atualizar roleManagement
description: Atualiza as propriedades de um objeto roleManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bb20f866db80486884779bca7d3a299c0352c1f8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685531"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="0bd89-103">Atualizar roleManagement</span><span class="sxs-lookup"><span data-stu-id="0bd89-103">Update roleManagement</span></span>

<span data-ttu-id="0bd89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bd89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bd89-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0bd89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bd89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0bd89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bd89-107">Atualiza as propriedades de um objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="0bd89-107">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bd89-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bd89-108">Prerequisites</span></span>
<span data-ttu-id="0bd89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bd89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bd89-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bd89-111">Permission type</span></span>|<span data-ttu-id="0bd89-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0bd89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bd89-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bd89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bd89-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bd89-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0bd89-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bd89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bd89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bd89-116">Not supported.</span></span>|
|<span data-ttu-id="0bd89-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bd89-117">Application</span></span>|<span data-ttu-id="0bd89-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bd89-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bd89-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bd89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="0bd89-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bd89-120">Request headers</span></span>
|<span data-ttu-id="0bd89-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bd89-121">Header</span></span>|<span data-ttu-id="0bd89-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0bd89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bd89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bd89-123">Authorization</span></span>|<span data-ttu-id="0bd89-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bd89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bd89-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bd89-125">Accept</span></span>|<span data-ttu-id="0bd89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bd89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bd89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bd89-127">Request body</span></span>
<span data-ttu-id="0bd89-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="0bd89-128">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="0bd89-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleManagement](../resources/intune-rbac-rolemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="0bd89-129">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="0bd89-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bd89-130">Property</span></span>|<span data-ttu-id="0bd89-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bd89-131">Type</span></span>|<span data-ttu-id="0bd89-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bd89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bd89-133">id</span><span class="sxs-lookup"><span data-stu-id="0bd89-133">id</span></span>|<span data-ttu-id="0bd89-134">String</span><span class="sxs-lookup"><span data-stu-id="0bd89-134">String</span></span>|<span data-ttu-id="0bd89-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0bd89-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0bd89-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bd89-136">Response</span></span>
<span data-ttu-id="0bd89-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bd89-137">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bd89-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bd89-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bd89-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bd89-139">Request</span></span>
<span data-ttu-id="0bd89-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bd89-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="0bd89-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bd89-141">Response</span></span>
<span data-ttu-id="0bd89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bd89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```





