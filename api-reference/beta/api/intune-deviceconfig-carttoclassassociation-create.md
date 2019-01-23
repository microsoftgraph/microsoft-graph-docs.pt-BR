---
title: Criar cartToClassAssociation
description: Crie um novo objeto de cartToClassAssociation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2368507adbf7e0065b10d4c0c93353d81d5d936
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423668"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="9cf55-103">Criar cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="9cf55-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="9cf55-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9cf55-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cf55-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9cf55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cf55-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9cf55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf55-107">Crie um novo objeto de [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="9cf55-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cf55-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9cf55-108">Prerequisites</span></span>
<span data-ttu-id="9cf55-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9cf55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9cf55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cf55-111">Permission type</span></span>|<span data-ttu-id="9cf55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9cf55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cf55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cf55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cf55-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf55-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cf55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cf55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cf55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cf55-116">Not supported.</span></span>|
|<span data-ttu-id="9cf55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cf55-117">Application</span></span>|<span data-ttu-id="9cf55-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cf55-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cf55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="9cf55-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf55-120">Request headers</span></span>
|<span data-ttu-id="9cf55-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9cf55-121">Header</span></span>|<span data-ttu-id="9cf55-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9cf55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cf55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cf55-123">Authorization</span></span>|<span data-ttu-id="9cf55-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cf55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cf55-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9cf55-125">Accept</span></span>|<span data-ttu-id="9cf55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cf55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cf55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf55-127">Request body</span></span>
<span data-ttu-id="9cf55-128">No corpo da solicitação, fornece uma representação JSON para o objeto cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="9cf55-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="9cf55-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="9cf55-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="9cf55-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cf55-130">Property</span></span>|<span data-ttu-id="9cf55-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf55-131">Type</span></span>|<span data-ttu-id="9cf55-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf55-133">id</span><span class="sxs-lookup"><span data-stu-id="9cf55-133">id</span></span>|<span data-ttu-id="9cf55-134">String</span><span class="sxs-lookup"><span data-stu-id="9cf55-134">String</span></span>|<span data-ttu-id="9cf55-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9cf55-135">Key of the entity.</span></span>|
|<span data-ttu-id="9cf55-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9cf55-136">createdDateTime</span></span>|<span data-ttu-id="9cf55-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cf55-137">DateTimeOffset</span></span>|<span data-ttu-id="9cf55-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9cf55-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="9cf55-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cf55-139">lastModifiedDateTime</span></span>|<span data-ttu-id="9cf55-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cf55-140">DateTimeOffset</span></span>|<span data-ttu-id="9cf55-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9cf55-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9cf55-142">version</span><span class="sxs-lookup"><span data-stu-id="9cf55-142">version</span></span>|<span data-ttu-id="9cf55-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf55-143">Int32</span></span>|<span data-ttu-id="9cf55-144">Versão do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="9cf55-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="9cf55-145">displayName</span><span class="sxs-lookup"><span data-stu-id="9cf55-145">displayName</span></span>|<span data-ttu-id="9cf55-146">String</span><span class="sxs-lookup"><span data-stu-id="9cf55-146">String</span></span>|<span data-ttu-id="9cf55-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9cf55-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="9cf55-148">description</span><span class="sxs-lookup"><span data-stu-id="9cf55-148">description</span></span>|<span data-ttu-id="9cf55-149">String</span><span class="sxs-lookup"><span data-stu-id="9cf55-149">String</span></span>|<span data-ttu-id="9cf55-150">Admin fornecido descrição do que o CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="9cf55-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="9cf55-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="9cf55-151">deviceCartIds</span></span>|<span data-ttu-id="9cf55-152">String collection</span><span class="sxs-lookup"><span data-stu-id="9cf55-152">String collection</span></span>|<span data-ttu-id="9cf55-153">Identificadores de carrinhos de dispositivo a ser associado a classes.</span><span class="sxs-lookup"><span data-stu-id="9cf55-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="9cf55-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="9cf55-154">classroomIds</span></span>|<span data-ttu-id="9cf55-155">String collection</span><span class="sxs-lookup"><span data-stu-id="9cf55-155">String collection</span></span>|<span data-ttu-id="9cf55-156">Identificadores de salas a ser associado ao dispositivo carrinhos de.</span><span class="sxs-lookup"><span data-stu-id="9cf55-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="9cf55-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf55-157">Response</span></span>
<span data-ttu-id="9cf55-158">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cf55-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf55-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cf55-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cf55-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf55-160">Request</span></span>
<span data-ttu-id="9cf55-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cf55-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9cf55-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf55-162">Response</span></span>
<span data-ttu-id="9cf55-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cf55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




