---
title: Criar windowsPhoneXAP
description: Criar um novo objeto windowsPhoneXAP.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6631eb2f4e9b755509052eb8f2297dc449baa99d
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790032"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="bc761-103">Criar windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="bc761-103">Create windowsPhoneXAP</span></span>

<span data-ttu-id="bc761-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc761-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc761-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc761-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc761-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc761-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc761-107">Criar um novo objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="bc761-107">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc761-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc761-108">Prerequisites</span></span>
<span data-ttu-id="bc761-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc761-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc761-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc761-111">Permission type</span></span>|<span data-ttu-id="bc761-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc761-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc761-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc761-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc761-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc761-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bc761-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc761-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc761-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc761-116">Not supported.</span></span>|
|<span data-ttu-id="bc761-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc761-117">Application</span></span>|<span data-ttu-id="bc761-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc761-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc761-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc761-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bc761-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc761-120">Request headers</span></span>
|<span data-ttu-id="bc761-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc761-121">Header</span></span>|<span data-ttu-id="bc761-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bc761-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc761-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc761-123">Authorization</span></span>|<span data-ttu-id="bc761-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc761-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc761-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc761-125">Accept</span></span>|<span data-ttu-id="bc761-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc761-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc761-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc761-127">Request body</span></span>
<span data-ttu-id="bc761-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhoneXAP.</span><span class="sxs-lookup"><span data-stu-id="bc761-128">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="bc761-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhoneXAP.</span><span class="sxs-lookup"><span data-stu-id="bc761-129">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="bc761-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc761-130">Property</span></span>|<span data-ttu-id="bc761-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc761-131">Type</span></span>|<span data-ttu-id="bc761-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc761-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc761-133">id</span><span class="sxs-lookup"><span data-stu-id="bc761-133">id</span></span>|<span data-ttu-id="bc761-134">String</span><span class="sxs-lookup"><span data-stu-id="bc761-134">String</span></span>|<span data-ttu-id="bc761-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc761-135">Key of the entity.</span></span> <span data-ttu-id="bc761-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bc761-137">displayName</span></span>|<span data-ttu-id="bc761-138">String</span><span class="sxs-lookup"><span data-stu-id="bc761-138">String</span></span>|<span data-ttu-id="bc761-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bc761-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bc761-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-141">description</span><span class="sxs-lookup"><span data-stu-id="bc761-141">description</span></span>|<span data-ttu-id="bc761-142">String</span><span class="sxs-lookup"><span data-stu-id="bc761-142">String</span></span>|<span data-ttu-id="bc761-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc761-143">The description of the app.</span></span> <span data-ttu-id="bc761-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-145">publicador</span><span class="sxs-lookup"><span data-stu-id="bc761-145">publisher</span></span>|<span data-ttu-id="bc761-146">String</span><span class="sxs-lookup"><span data-stu-id="bc761-146">String</span></span>|<span data-ttu-id="bc761-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc761-147">The publisher of the app.</span></span> <span data-ttu-id="bc761-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bc761-149">largeIcon</span></span>|[<span data-ttu-id="bc761-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bc761-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bc761-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bc761-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bc761-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc761-153">createdDateTime</span></span>|<span data-ttu-id="bc761-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc761-154">DateTimeOffset</span></span>|<span data-ttu-id="bc761-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc761-155">The date and time the app was created.</span></span> <span data-ttu-id="bc761-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc761-157">lastModifiedDateTime</span></span>|<span data-ttu-id="bc761-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc761-158">DateTimeOffset</span></span>|<span data-ttu-id="bc761-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bc761-159">The date and time the app was last modified.</span></span> <span data-ttu-id="bc761-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bc761-161">isFeatured</span></span>|<span data-ttu-id="bc761-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc761-162">Boolean</span></span>|<span data-ttu-id="bc761-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bc761-164">privacyInformationUrl</span></span>|<span data-ttu-id="bc761-165">String</span><span class="sxs-lookup"><span data-stu-id="bc761-165">String</span></span>|<span data-ttu-id="bc761-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bc761-166">The privacy statement Url.</span></span> <span data-ttu-id="bc761-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bc761-168">informationUrl</span></span>|<span data-ttu-id="bc761-169">String</span><span class="sxs-lookup"><span data-stu-id="bc761-169">String</span></span>|<span data-ttu-id="bc761-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bc761-170">The more information Url.</span></span> <span data-ttu-id="bc761-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-172">owner</span><span class="sxs-lookup"><span data-stu-id="bc761-172">owner</span></span>|<span data-ttu-id="bc761-173">String</span><span class="sxs-lookup"><span data-stu-id="bc761-173">String</span></span>|<span data-ttu-id="bc761-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bc761-174">The owner of the app.</span></span> <span data-ttu-id="bc761-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-176">developer</span><span class="sxs-lookup"><span data-stu-id="bc761-176">developer</span></span>|<span data-ttu-id="bc761-177">String</span><span class="sxs-lookup"><span data-stu-id="bc761-177">String</span></span>|<span data-ttu-id="bc761-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc761-178">The developer of the app.</span></span> <span data-ttu-id="bc761-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-180">notes</span><span class="sxs-lookup"><span data-stu-id="bc761-180">notes</span></span>|<span data-ttu-id="bc761-181">String</span><span class="sxs-lookup"><span data-stu-id="bc761-181">String</span></span>|<span data-ttu-id="bc761-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc761-182">Notes for the app.</span></span> <span data-ttu-id="bc761-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="bc761-184">uploadState</span></span>|<span data-ttu-id="bc761-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bc761-185">Int32</span></span>|<span data-ttu-id="bc761-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="bc761-186">The upload state.</span></span> <span data-ttu-id="bc761-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="bc761-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="bc761-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="bc761-189">publishingState</span></span>|[<span data-ttu-id="bc761-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bc761-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bc761-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc761-191">The publishing state for the app.</span></span> <span data-ttu-id="bc761-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="bc761-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bc761-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc761-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bc761-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bc761-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bc761-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bc761-195">isAssigned</span></span>|<span data-ttu-id="bc761-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc761-196">Boolean</span></span>|<span data-ttu-id="bc761-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="bc761-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bc761-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc761-199">roleScopeTagIds</span></span>|<span data-ttu-id="bc761-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc761-200">String collection</span></span>|<span data-ttu-id="bc761-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="bc761-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bc761-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="bc761-203">dependentAppCount</span></span>|<span data-ttu-id="bc761-204">Int32</span><span class="sxs-lookup"><span data-stu-id="bc761-204">Int32</span></span>|<span data-ttu-id="bc761-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="bc761-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bc761-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bc761-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bc761-207">committedContentVersion</span></span>|<span data-ttu-id="bc761-208">String</span><span class="sxs-lookup"><span data-stu-id="bc761-208">String</span></span>|<span data-ttu-id="bc761-209">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="bc761-209">The internal committed content version.</span></span> <span data-ttu-id="bc761-210">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc761-211">fileName</span><span class="sxs-lookup"><span data-stu-id="bc761-211">fileName</span></span>|<span data-ttu-id="bc761-212">String</span><span class="sxs-lookup"><span data-stu-id="bc761-212">String</span></span>|<span data-ttu-id="bc761-213">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="bc761-213">The name of the main Lob application file.</span></span> <span data-ttu-id="bc761-214">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc761-215">size</span><span class="sxs-lookup"><span data-stu-id="bc761-215">size</span></span>|<span data-ttu-id="bc761-216">Int64</span><span class="sxs-lookup"><span data-stu-id="bc761-216">Int64</span></span>|<span data-ttu-id="bc761-217">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="bc761-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="bc761-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc761-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc761-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc761-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bc761-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc761-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="bc761-221">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="bc761-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bc761-222">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc761-222">productIdentifier</span></span>|<span data-ttu-id="bc761-223">String</span><span class="sxs-lookup"><span data-stu-id="bc761-223">String</span></span>|<span data-ttu-id="bc761-224">O identificador do produto.</span><span class="sxs-lookup"><span data-stu-id="bc761-224">The Product Identifier.</span></span>|
|<span data-ttu-id="bc761-225">identityVersion</span><span class="sxs-lookup"><span data-stu-id="bc761-225">identityVersion</span></span>|<span data-ttu-id="bc761-226">String</span><span class="sxs-lookup"><span data-stu-id="bc761-226">String</span></span>|<span data-ttu-id="bc761-227">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="bc761-227">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="bc761-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc761-228">Response</span></span>
<span data-ttu-id="bc761-229">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc761-229">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc761-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc761-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc761-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc761-231">Request</span></span>
<span data-ttu-id="bc761-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc761-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc761-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc761-233">Response</span></span>
<span data-ttu-id="bc761-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc761-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



