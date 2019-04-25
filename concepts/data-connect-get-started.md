---
title: Introdução ao Microsoft Graph Data Connect (versão prévia)
description: 'Antes de poder usar o Microsoft Graph Data Connect, um administrador do Office 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management). '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: f7426147908a2ded298bee065c05afffc182cd4b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526116"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a><span data-ttu-id="b4563-103">Introdução ao Microsoft Graph Data Connect (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="b4563-103">Get started with Microsoft Graph data connect (preview)</span></span>

<span data-ttu-id="b4563-104">Antes de poder usar o Microsoft Graph Data Connect, um administrador do Office 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management).</span><span class="sxs-lookup"><span data-stu-id="b4563-104">Before you can use Microsoft Graph data connect, an Office 365 administrator must take two actions, both of which enable the ability for the admin to control data movement through Privileged Access Management (PAM).</span></span> 

1. <span data-ttu-id="b4563-105">Dê consentimento à aceitação do Microsoft Graph Data Connect por meio do Portal de Administração do Microsoft 365, na página **Serviços e suplementos**.</span><span class="sxs-lookup"><span data-stu-id="b4563-105">Give consent to opt in to Microsoft Graph data connect through the Microsoft 365 Admin Portal, on the **Services & add-ins** page.</span></span> <span data-ttu-id="b4563-106">Isso permitirá solicitações de movimentação de dados no Microsoft Azure (ou seja, manter o controle total sobre os dados, mas permitir que os recursos do Azure os acessem).</span><span class="sxs-lookup"><span data-stu-id="b4563-106">This will allow data movement requests to Microsoft Azure (that is, keep full control over the data, but allow Azure resources to access it).</span></span> <span data-ttu-id="b4563-107">Nenhum dado é transferido, a menos que aprovação de um pipeline específico seja fornecida mais tarde.</span><span class="sxs-lookup"><span data-stu-id="b4563-107">No data is transferred unless approval for a specific pipeline is provided later.</span></span>
2. <span data-ttu-id="b4563-108">Configure um grupo aprovador dentro da assinatura do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b4563-108">Set an approver group within the Office 365 subscription.</span></span> <span data-ttu-id="b4563-109">Verifique se o grupo aprovador não está vazio.</span><span class="sxs-lookup"><span data-stu-id="b4563-109">Make sure that the approver group is not empty.</span></span> <span data-ttu-id="b4563-110">Somente os usuários no grupo podem aprovar solicitações de movimentação de dados.</span><span class="sxs-lookup"><span data-stu-id="b4563-110">Only the users in the group can approve data movement requests.</span></span>

<span data-ttu-id="b4563-111">Para obter instruções passo a passo, veja o [módulo de treinamento do Microsoft Graph Data Connect](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span><span class="sxs-lookup"><span data-stu-id="b4563-111">For detailed step-by-step instructions, see the [Microsoft Graph data connect training module](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="b4563-112">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b4563-112">Next steps</span></span>

<span data-ttu-id="b4563-113">Parabéns!</span><span class="sxs-lookup"><span data-stu-id="b4563-113">Congratulations!</span></span> <span data-ttu-id="b4563-114">Agora você está pronto para começar a criar aplicativos inteligentes com as ferramentas do Azure.</span><span class="sxs-lookup"><span data-stu-id="b4563-114">You're now ready to start building intelligent applications with Azure tooling.</span></span> <span data-ttu-id="b4563-115">Para documentação adicional e um aplicativo de exemplo, veja o [repositório do GitHub do Microsoft Graph Data Connect](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).</span><span class="sxs-lookup"><span data-stu-id="b4563-115">For a sample application and additional documentation, see the [Microsoft Graph data connect GitHub repo](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).</span></span> 
