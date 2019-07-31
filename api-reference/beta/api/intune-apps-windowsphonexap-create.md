---
title: Criar windowsPhoneXAP
description: Criar um novo objeto windowsPhoneXAP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd38f3d66bd77dc5a6383bd51ab603f5e63f814b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959842"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="2f2d1-103">Criar windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="2f2d1-103">Create windowsPhoneXAP</span></span>

> <span data-ttu-id="2f2d1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f2d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f2d1-106">Criar um novo objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="2f2d1-106">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f2d1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f2d1-107">Prerequisites</span></span>
<span data-ttu-id="2f2d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f2d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f2d1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f2d1-110">Permission type</span></span>|<span data-ttu-id="2f2d1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f2d1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f2d1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2d1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f2d1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f2d1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-115">Not supported.</span></span>|
|<span data-ttu-id="2f2d1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f2d1-116">Application</span></span>|<span data-ttu-id="2f2d1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f2d1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f2d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2f2d1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2d1-119">Request headers</span></span>
|<span data-ttu-id="2f2d1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f2d1-120">Header</span></span>|<span data-ttu-id="2f2d1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f2d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f2d1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f2d1-122">Authorization</span></span>|<span data-ttu-id="2f2d1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f2d1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f2d1-124">Accept</span></span>|<span data-ttu-id="2f2d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f2d1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2d1-126">Request body</span></span>
<span data-ttu-id="2f2d1-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhoneXAP.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-127">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="2f2d1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhoneXAP.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-128">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="2f2d1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f2d1-129">Property</span></span>|<span data-ttu-id="2f2d1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f2d1-130">Type</span></span>|<span data-ttu-id="2f2d1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f2d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f2d1-132">id</span><span class="sxs-lookup"><span data-stu-id="2f2d1-132">id</span></span>|<span data-ttu-id="2f2d1-133">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-133">String</span></span>|<span data-ttu-id="2f2d1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-134">Key of the entity.</span></span> <span data-ttu-id="2f2d1-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2f2d1-136">displayName</span></span>|<span data-ttu-id="2f2d1-137">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-137">String</span></span>|<span data-ttu-id="2f2d1-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2f2d1-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-140">descrição</span><span class="sxs-lookup"><span data-stu-id="2f2d1-140">description</span></span>|<span data-ttu-id="2f2d1-141">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-141">String</span></span>|<span data-ttu-id="2f2d1-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-142">The description of the app.</span></span> <span data-ttu-id="2f2d1-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-144">publicador</span><span class="sxs-lookup"><span data-stu-id="2f2d1-144">publisher</span></span>|<span data-ttu-id="2f2d1-145">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-145">String</span></span>|<span data-ttu-id="2f2d1-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-146">The publisher of the app.</span></span> <span data-ttu-id="2f2d1-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2f2d1-148">largeIcon</span></span>|[<span data-ttu-id="2f2d1-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2f2d1-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2f2d1-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2f2d1-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f2d1-152">createdDateTime</span></span>|<span data-ttu-id="2f2d1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f2d1-153">DateTimeOffset</span></span>|<span data-ttu-id="2f2d1-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-154">The date and time the app was created.</span></span> <span data-ttu-id="2f2d1-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f2d1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2f2d1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f2d1-157">DateTimeOffset</span></span>|<span data-ttu-id="2f2d1-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2f2d1-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2f2d1-160">isFeatured</span></span>|<span data-ttu-id="2f2d1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f2d1-161">Boolean</span></span>|<span data-ttu-id="2f2d1-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2f2d1-163">privacyInformationUrl</span></span>|<span data-ttu-id="2f2d1-164">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-164">String</span></span>|<span data-ttu-id="2f2d1-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-165">The privacy statement Url.</span></span> <span data-ttu-id="2f2d1-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2f2d1-167">informationUrl</span></span>|<span data-ttu-id="2f2d1-168">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-168">String</span></span>|<span data-ttu-id="2f2d1-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-169">The more information Url.</span></span> <span data-ttu-id="2f2d1-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-171">owner</span><span class="sxs-lookup"><span data-stu-id="2f2d1-171">owner</span></span>|<span data-ttu-id="2f2d1-172">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-172">String</span></span>|<span data-ttu-id="2f2d1-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-173">The owner of the app.</span></span> <span data-ttu-id="2f2d1-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-175">developer</span><span class="sxs-lookup"><span data-stu-id="2f2d1-175">developer</span></span>|<span data-ttu-id="2f2d1-176">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-176">String</span></span>|<span data-ttu-id="2f2d1-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-177">The developer of the app.</span></span> <span data-ttu-id="2f2d1-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-179">notes</span><span class="sxs-lookup"><span data-stu-id="2f2d1-179">notes</span></span>|<span data-ttu-id="2f2d1-180">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-180">String</span></span>|<span data-ttu-id="2f2d1-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-181">Notes for the app.</span></span> <span data-ttu-id="2f2d1-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2f2d1-183">uploadState</span></span>|<span data-ttu-id="2f2d1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2d1-184">Int32</span></span>|<span data-ttu-id="2f2d1-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-185">The upload state.</span></span> <span data-ttu-id="2f2d1-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2f2d1-187">publishingState</span></span>|[<span data-ttu-id="2f2d1-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2f2d1-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2f2d1-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-189">The publishing state for the app.</span></span> <span data-ttu-id="2f2d1-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2f2d1-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f2d1-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2f2d1-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2f2d1-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2f2d1-193">isAssigned</span></span>|<span data-ttu-id="2f2d1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f2d1-194">Boolean</span></span>|<span data-ttu-id="2f2d1-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2f2d1-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f2d1-197">roleScopeTagIds</span></span>|<span data-ttu-id="2f2d1-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f2d1-198">String collection</span></span>|<span data-ttu-id="2f2d1-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2f2d1-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2f2d1-201">dependentAppCount</span></span>|<span data-ttu-id="2f2d1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2d1-202">Int32</span></span>|<span data-ttu-id="2f2d1-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2f2d1-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f2d1-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2f2d1-205">committedContentVersion</span></span>|<span data-ttu-id="2f2d1-206">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-206">String</span></span>|<span data-ttu-id="2f2d1-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-207">The internal committed content version.</span></span> <span data-ttu-id="2f2d1-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2f2d1-209">fileName</span><span class="sxs-lookup"><span data-stu-id="2f2d1-209">fileName</span></span>|<span data-ttu-id="2f2d1-210">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-210">String</span></span>|<span data-ttu-id="2f2d1-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-211">The name of the main Lob application file.</span></span> <span data-ttu-id="2f2d1-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2f2d1-213">size</span><span class="sxs-lookup"><span data-stu-id="2f2d1-213">size</span></span>|<span data-ttu-id="2f2d1-214">Int64</span><span class="sxs-lookup"><span data-stu-id="2f2d1-214">Int64</span></span>|<span data-ttu-id="2f2d1-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="2f2d1-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d1-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2f2d1-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2f2d1-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2f2d1-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2f2d1-218">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2f2d1-219">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2f2d1-220">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f2d1-220">productIdentifier</span></span>|<span data-ttu-id="2f2d1-221">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-221">String</span></span>|<span data-ttu-id="2f2d1-222">O identificador do produto.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-222">The Product Identifier.</span></span>|
|<span data-ttu-id="2f2d1-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2f2d1-223">identityVersion</span></span>|<span data-ttu-id="2f2d1-224">String</span><span class="sxs-lookup"><span data-stu-id="2f2d1-224">String</span></span>|<span data-ttu-id="2f2d1-225">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2f2d1-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f2d1-226">Response</span></span>
<span data-ttu-id="2f2d1-227">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-227">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f2d1-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f2d1-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f2d1-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2d1-229">Request</span></span>
<span data-ttu-id="2f2d1-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="2f2d1-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f2d1-231">Response</span></span>
<span data-ttu-id="2f2d1-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f2d1-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





