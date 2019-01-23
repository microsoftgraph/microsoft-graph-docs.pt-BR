---
title: Criar windowsMobileMSI
description: Cria um novo objeto windowsMobileMSI.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a794ea35428b606c825dc95de3a76aa839708489
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405111"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="81a84-103">Criar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="81a84-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="81a84-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="81a84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81a84-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="81a84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81a84-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="81a84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a84-107">Cria um novo objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="81a84-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81a84-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81a84-108">Prerequisites</span></span>
<span data-ttu-id="81a84-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="81a84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="81a84-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81a84-111">Permission type</span></span>|<span data-ttu-id="81a84-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81a84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81a84-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81a84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81a84-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81a84-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81a84-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81a84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81a84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a84-116">Not supported.</span></span>|
|<span data-ttu-id="81a84-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81a84-117">Application</span></span>|<span data-ttu-id="81a84-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81a84-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81a84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="81a84-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81a84-120">Request headers</span></span>
|<span data-ttu-id="81a84-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81a84-121">Header</span></span>|<span data-ttu-id="81a84-122">Valor</span><span class="sxs-lookup"><span data-stu-id="81a84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81a84-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81a84-123">Authorization</span></span>|<span data-ttu-id="81a84-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81a84-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81a84-125">Accept</span></span>|<span data-ttu-id="81a84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81a84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a84-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81a84-127">Request body</span></span>
<span data-ttu-id="81a84-128">No corpo da solicitação, forneça uma representação JSON para o objeto windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="81a84-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="81a84-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="81a84-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="81a84-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81a84-130">Property</span></span>|<span data-ttu-id="81a84-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="81a84-131">Type</span></span>|<span data-ttu-id="81a84-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="81a84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a84-133">id</span><span class="sxs-lookup"><span data-stu-id="81a84-133">id</span></span>|<span data-ttu-id="81a84-134">String</span><span class="sxs-lookup"><span data-stu-id="81a84-134">String</span></span>|<span data-ttu-id="81a84-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="81a84-135">Key of the entity.</span></span> <span data-ttu-id="81a84-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-137">displayName</span><span class="sxs-lookup"><span data-stu-id="81a84-137">displayName</span></span>|<span data-ttu-id="81a84-138">String</span><span class="sxs-lookup"><span data-stu-id="81a84-138">String</span></span>|<span data-ttu-id="81a84-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="81a84-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="81a84-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-141">description</span><span class="sxs-lookup"><span data-stu-id="81a84-141">description</span></span>|<span data-ttu-id="81a84-142">String</span><span class="sxs-lookup"><span data-stu-id="81a84-142">String</span></span>|<span data-ttu-id="81a84-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81a84-143">The description of the app.</span></span> <span data-ttu-id="81a84-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-145">publisher</span><span class="sxs-lookup"><span data-stu-id="81a84-145">publisher</span></span>|<span data-ttu-id="81a84-146">String</span><span class="sxs-lookup"><span data-stu-id="81a84-146">String</span></span>|<span data-ttu-id="81a84-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81a84-147">The publisher of the app.</span></span> <span data-ttu-id="81a84-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="81a84-149">largeIcon</span></span>|[<span data-ttu-id="81a84-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="81a84-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="81a84-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="81a84-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="81a84-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81a84-153">createdDateTime</span></span>|<span data-ttu-id="81a84-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a84-154">DateTimeOffset</span></span>|<span data-ttu-id="81a84-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81a84-155">The date and time the app was created.</span></span> <span data-ttu-id="81a84-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81a84-157">lastModifiedDateTime</span></span>|<span data-ttu-id="81a84-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a84-158">DateTimeOffset</span></span>|<span data-ttu-id="81a84-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="81a84-159">The date and time the app was last modified.</span></span> <span data-ttu-id="81a84-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="81a84-161">isFeatured</span></span>|<span data-ttu-id="81a84-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="81a84-162">Boolean</span></span>|<span data-ttu-id="81a84-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="81a84-164">privacyInformationUrl</span></span>|<span data-ttu-id="81a84-165">String</span><span class="sxs-lookup"><span data-stu-id="81a84-165">String</span></span>|<span data-ttu-id="81a84-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="81a84-166">The privacy statement Url.</span></span> <span data-ttu-id="81a84-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="81a84-168">informationUrl</span></span>|<span data-ttu-id="81a84-169">String</span><span class="sxs-lookup"><span data-stu-id="81a84-169">String</span></span>|<span data-ttu-id="81a84-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="81a84-170">The more information Url.</span></span> <span data-ttu-id="81a84-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-172">owner</span><span class="sxs-lookup"><span data-stu-id="81a84-172">owner</span></span>|<span data-ttu-id="81a84-173">String</span><span class="sxs-lookup"><span data-stu-id="81a84-173">String</span></span>|<span data-ttu-id="81a84-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="81a84-174">The owner of the app.</span></span> <span data-ttu-id="81a84-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-176">developer</span><span class="sxs-lookup"><span data-stu-id="81a84-176">developer</span></span>|<span data-ttu-id="81a84-177">String</span><span class="sxs-lookup"><span data-stu-id="81a84-177">String</span></span>|<span data-ttu-id="81a84-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81a84-178">The developer of the app.</span></span> <span data-ttu-id="81a84-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-180">Observações</span><span class="sxs-lookup"><span data-stu-id="81a84-180">notes</span></span>|<span data-ttu-id="81a84-181">String</span><span class="sxs-lookup"><span data-stu-id="81a84-181">String</span></span>|<span data-ttu-id="81a84-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81a84-182">Notes for the app.</span></span> <span data-ttu-id="81a84-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="81a84-184">uploadState</span></span>|<span data-ttu-id="81a84-185">Int32</span><span class="sxs-lookup"><span data-stu-id="81a84-185">Int32</span></span>|<span data-ttu-id="81a84-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="81a84-186">The upload state.</span></span> <span data-ttu-id="81a84-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="81a84-188">publishingState</span></span>|[<span data-ttu-id="81a84-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="81a84-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="81a84-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81a84-190">The publishing state for the app.</span></span> <span data-ttu-id="81a84-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="81a84-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="81a84-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="81a84-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="81a84-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="81a84-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="81a84-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="81a84-194">isAssigned</span></span>|<span data-ttu-id="81a84-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="81a84-195">Boolean</span></span>|<span data-ttu-id="81a84-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="81a84-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="81a84-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81a84-198">roleScopeTagIds</span></span>|<span data-ttu-id="81a84-199">String collection</span><span class="sxs-lookup"><span data-stu-id="81a84-199">String collection</span></span>|<span data-ttu-id="81a84-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="81a84-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="81a84-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81a84-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="81a84-202">committedContentVersion</span></span>|<span data-ttu-id="81a84-203">String</span><span class="sxs-lookup"><span data-stu-id="81a84-203">String</span></span>|<span data-ttu-id="81a84-204">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="81a84-204">The internal committed content version.</span></span> <span data-ttu-id="81a84-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="81a84-206">fileName</span><span class="sxs-lookup"><span data-stu-id="81a84-206">fileName</span></span>|<span data-ttu-id="81a84-207">String</span><span class="sxs-lookup"><span data-stu-id="81a84-207">String</span></span>|<span data-ttu-id="81a84-208">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="81a84-208">The name of the main Lob application file.</span></span> <span data-ttu-id="81a84-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="81a84-210">size</span><span class="sxs-lookup"><span data-stu-id="81a84-210">size</span></span>|<span data-ttu-id="81a84-211">Int64</span><span class="sxs-lookup"><span data-stu-id="81a84-211">Int64</span></span>|<span data-ttu-id="81a84-212">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="81a84-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="81a84-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="81a84-214">commandLine</span><span class="sxs-lookup"><span data-stu-id="81a84-214">commandLine</span></span>|<span data-ttu-id="81a84-215">String</span><span class="sxs-lookup"><span data-stu-id="81a84-215">String</span></span>|<span data-ttu-id="81a84-216">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="81a84-216">The command line.</span></span>|
|<span data-ttu-id="81a84-217">productCode</span><span class="sxs-lookup"><span data-stu-id="81a84-217">productCode</span></span>|<span data-ttu-id="81a84-218">String</span><span class="sxs-lookup"><span data-stu-id="81a84-218">String</span></span>|<span data-ttu-id="81a84-219">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="81a84-219">The product code.</span></span>|
|<span data-ttu-id="81a84-220">productVersion</span><span class="sxs-lookup"><span data-stu-id="81a84-220">productVersion</span></span>|<span data-ttu-id="81a84-221">String</span><span class="sxs-lookup"><span data-stu-id="81a84-221">String</span></span>|<span data-ttu-id="81a84-222">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="81a84-222">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="81a84-223">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="81a84-223">ignoreVersionDetection</span></span>|<span data-ttu-id="81a84-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="81a84-224">Boolean</span></span>|<span data-ttu-id="81a84-225">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81a84-225">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="81a84-226">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="81a84-226">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="81a84-227">identityVersion</span><span class="sxs-lookup"><span data-stu-id="81a84-227">identityVersion</span></span>|<span data-ttu-id="81a84-228">String</span><span class="sxs-lookup"><span data-stu-id="81a84-228">String</span></span>|<span data-ttu-id="81a84-229">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="81a84-229">The identity version.</span></span>|
|<span data-ttu-id="81a84-230">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="81a84-230">useDeviceContext</span></span>|<span data-ttu-id="81a84-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="81a84-231">Boolean</span></span>|<span data-ttu-id="81a84-232">Indica se a instalação MSI um modo duplo no contexto do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81a84-232">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="81a84-233">Se for true, aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="81a84-233">If true, app will be installed for all users.</span></span> <span data-ttu-id="81a84-234">Se for false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="81a84-234">If false, app will be installed per-user.</span></span> <span data-ttu-id="81a84-235">Se for null, serviço usará o contexto de instalação do pacote MSI padrão.</span><span class="sxs-lookup"><span data-stu-id="81a84-235">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="81a84-236">Em caso de modo duplo MSI, esse padrão serão por usuário.</span><span class="sxs-lookup"><span data-stu-id="81a84-236">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="81a84-237">Não podem ser definidas para aplicativos de modo não-duplo.</span><span class="sxs-lookup"><span data-stu-id="81a84-237">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="81a84-238">Não pode ser alterada após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81a84-238">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="81a84-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a84-239">Response</span></span>
<span data-ttu-id="81a84-240">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81a84-240">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81a84-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81a84-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="81a84-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81a84-242">Request</span></span>
<span data-ttu-id="81a84-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81a84-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="81a84-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a84-244">Response</span></span>
<span data-ttu-id="81a84-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81a84-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




