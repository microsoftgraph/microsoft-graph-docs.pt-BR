---
title: Criar cartToClassAssociation
description: Criar um novo objeto cartToClassAssociation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 365b2f7ac94c3b8c5583f6fa3106341b882d28cf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722675"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="ca595-103">Criar cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="ca595-103">Create cartToClassAssociation</span></span>

<span data-ttu-id="ca595-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca595-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca595-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca595-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca595-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca595-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca595-107">Criar um novo objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="ca595-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca595-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca595-108">Prerequisites</span></span>
<span data-ttu-id="ca595-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca595-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca595-111">Permission type</span></span>|<span data-ttu-id="ca595-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca595-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca595-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca595-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca595-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca595-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca595-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca595-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca595-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca595-116">Not supported.</span></span>|
|<span data-ttu-id="ca595-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca595-117">Application</span></span>|<span data-ttu-id="ca595-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca595-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca595-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca595-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="ca595-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca595-120">Request headers</span></span>
|<span data-ttu-id="ca595-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca595-121">Header</span></span>|<span data-ttu-id="ca595-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca595-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca595-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca595-123">Authorization</span></span>|<span data-ttu-id="ca595-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca595-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca595-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca595-125">Accept</span></span>|<span data-ttu-id="ca595-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca595-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca595-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca595-127">Request body</span></span>
<span data-ttu-id="ca595-128">No corpo da solicitação, forneça uma representação JSON do objeto cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="ca595-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="ca595-129">A tabela a seguir mostra as propriedades que são necessárias ao criar cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="ca595-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="ca595-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca595-130">Property</span></span>|<span data-ttu-id="ca595-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca595-131">Type</span></span>|<span data-ttu-id="ca595-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca595-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca595-133">id</span><span class="sxs-lookup"><span data-stu-id="ca595-133">id</span></span>|<span data-ttu-id="ca595-134">String</span><span class="sxs-lookup"><span data-stu-id="ca595-134">String</span></span>|<span data-ttu-id="ca595-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca595-135">Key of the entity.</span></span>|
|<span data-ttu-id="ca595-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca595-136">createdDateTime</span></span>|<span data-ttu-id="ca595-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca595-137">DateTimeOffset</span></span>|<span data-ttu-id="ca595-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ca595-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="ca595-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca595-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ca595-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca595-140">DateTimeOffset</span></span>|<span data-ttu-id="ca595-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ca595-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ca595-142">versão</span><span class="sxs-lookup"><span data-stu-id="ca595-142">version</span></span>|<span data-ttu-id="ca595-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ca595-143">Int32</span></span>|<span data-ttu-id="ca595-144">Versão do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="ca595-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="ca595-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ca595-145">displayName</span></span>|<span data-ttu-id="ca595-146">String</span><span class="sxs-lookup"><span data-stu-id="ca595-146">String</span></span>|<span data-ttu-id="ca595-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca595-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ca595-148">description</span><span class="sxs-lookup"><span data-stu-id="ca595-148">description</span></span>|<span data-ttu-id="ca595-149">String</span><span class="sxs-lookup"><span data-stu-id="ca595-149">String</span></span>|<span data-ttu-id="ca595-150">Descrição fornecida pelo administrador do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="ca595-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="ca595-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="ca595-151">deviceCartIds</span></span>|<span data-ttu-id="ca595-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca595-152">String collection</span></span>|<span data-ttu-id="ca595-153">Identificadores de carrinhos de dispositivos a serem associados às classes.</span><span class="sxs-lookup"><span data-stu-id="ca595-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="ca595-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="ca595-154">classroomIds</span></span>|<span data-ttu-id="ca595-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca595-155">String collection</span></span>|<span data-ttu-id="ca595-156">Identificadores de salas de aula a serem associadas a carrinhos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ca595-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="ca595-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca595-157">Response</span></span>
<span data-ttu-id="ca595-158">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca595-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca595-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca595-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca595-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca595-160">Request</span></span>
<span data-ttu-id="ca595-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca595-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ca595-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca595-162">Response</span></span>
<span data-ttu-id="ca595-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca595-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





