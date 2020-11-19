---
title: Atualizar rbacApplicationMultiple
description: Atualiza as propriedades de um objeto rbacApplicationMultiple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 649ecc69a97213b3d94d41afcf970ff4ad73435f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257720"
---
# <a name="update-rbacapplicationmultiple"></a><span data-ttu-id="cb1c8-103">Atualizar rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="cb1c8-103">Update rbacApplicationMultiple</span></span>

<span data-ttu-id="cb1c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb1c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb1c8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb1c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb1c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb1c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb1c8-107">Atualiza as propriedades de um objeto [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="cb1c8-107">Update the properties of a [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb1c8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb1c8-108">Prerequisites</span></span>
<span data-ttu-id="cb1c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb1c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb1c8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb1c8-111">Permission type</span></span>|<span data-ttu-id="cb1c8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb1c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb1c8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb1c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb1c8-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb1c8-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cb1c8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb1c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb1c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb1c8-116">Not supported.</span></span>|
|<span data-ttu-id="cb1c8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb1c8-117">Application</span></span>|<span data-ttu-id="cb1c8-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb1c8-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb1c8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb1c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="cb1c8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb1c8-120">Request headers</span></span>
|<span data-ttu-id="cb1c8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb1c8-121">Header</span></span>|<span data-ttu-id="cb1c8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cb1c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb1c8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb1c8-123">Authorization</span></span>|<span data-ttu-id="cb1c8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb1c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb1c8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cb1c8-125">Accept</span></span>|<span data-ttu-id="cb1c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb1c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb1c8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb1c8-127">Request body</span></span>
<span data-ttu-id="cb1c8-128">No corpo da solicitação, forneça uma representação JSON do objeto [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="cb1c8-128">In the request body, supply a JSON representation for the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

<span data-ttu-id="cb1c8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span><span class="sxs-lookup"><span data-stu-id="cb1c8-129">The following table shows the properties that are required when you create the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span></span>

|<span data-ttu-id="cb1c8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb1c8-130">Property</span></span>|<span data-ttu-id="cb1c8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb1c8-131">Type</span></span>|<span data-ttu-id="cb1c8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb1c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb1c8-133">id</span><span class="sxs-lookup"><span data-stu-id="cb1c8-133">id</span></span>|<span data-ttu-id="cb1c8-134">String</span><span class="sxs-lookup"><span data-stu-id="cb1c8-134">String</span></span>|<span data-ttu-id="cb1c8-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cb1c8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cb1c8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb1c8-136">Response</span></span>
<span data-ttu-id="cb1c8-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb1c8-137">If successful, this method returns a `200 OK` response code and an updated [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb1c8-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb1c8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb1c8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb1c8-139">Request</span></span>
<span data-ttu-id="cb1c8-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb1c8-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### <a name="response"></a><span data-ttu-id="cb1c8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb1c8-141">Response</span></span>
<span data-ttu-id="cb1c8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb1c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "ee4797e5-97e5-ee47-e597-47eee59747ee"
}
```




