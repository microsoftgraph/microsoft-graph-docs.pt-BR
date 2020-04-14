---
title: Atualizar roleManagement
description: Atualiza as propriedades de um objeto roleManagement.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d81ccac5dc51c1193f6956c346910aa66784898
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423900"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="51bd5-103">Atualizar roleManagement</span><span class="sxs-lookup"><span data-stu-id="51bd5-103">Update roleManagement</span></span>

<span data-ttu-id="51bd5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51bd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51bd5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51bd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51bd5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51bd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51bd5-107">Atualiza as propriedades de um objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="51bd5-107">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51bd5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51bd5-108">Prerequisites</span></span>
<span data-ttu-id="51bd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51bd5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51bd5-111">Permission type</span></span>|<span data-ttu-id="51bd5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51bd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51bd5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51bd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51bd5-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51bd5-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="51bd5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51bd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51bd5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51bd5-116">Not supported.</span></span>|
|<span data-ttu-id="51bd5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51bd5-117">Application</span></span>|<span data-ttu-id="51bd5-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51bd5-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51bd5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51bd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="51bd5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51bd5-120">Request headers</span></span>
|<span data-ttu-id="51bd5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51bd5-121">Header</span></span>|<span data-ttu-id="51bd5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51bd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51bd5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51bd5-123">Authorization</span></span>|<span data-ttu-id="51bd5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51bd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51bd5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51bd5-125">Accept</span></span>|<span data-ttu-id="51bd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51bd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51bd5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51bd5-127">Request body</span></span>
<span data-ttu-id="51bd5-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="51bd5-128">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="51bd5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleManagement](../resources/intune-rbac-rolemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="51bd5-129">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="51bd5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51bd5-130">Property</span></span>|<span data-ttu-id="51bd5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="51bd5-131">Type</span></span>|<span data-ttu-id="51bd5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="51bd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51bd5-133">id</span><span class="sxs-lookup"><span data-stu-id="51bd5-133">id</span></span>|<span data-ttu-id="51bd5-134">String</span><span class="sxs-lookup"><span data-stu-id="51bd5-134">String</span></span>|<span data-ttu-id="51bd5-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51bd5-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="51bd5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="51bd5-136">Response</span></span>
<span data-ttu-id="51bd5-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51bd5-137">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51bd5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51bd5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="51bd5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51bd5-139">Request</span></span>
<span data-ttu-id="51bd5-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51bd5-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="51bd5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="51bd5-141">Response</span></span>
<span data-ttu-id="51bd5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51bd5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```



