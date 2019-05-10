---
title: Políticas e licença do Microsoft Graph Data Connect
description: Descreve quais políticas são compatíveis e como atribuir acesso ISV a SKUs para organizações.
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 2f96f099289346455a31ea42c4cb643eb997d558
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629912"
---
# <a name="microsoft-graph-data-connect-policies-and-licensing"></a>Políticas e licença do Microsoft Graph Data Connect

Microsoft Graph Data Connect utiliza [aplicativos gerenciados do Azure](https://docs.microsoft.com/pt-BR/azure/managed-applications/overview) para que você possa criar e implantar soluções em seu ambiente do cliente do Azure. Aplicativos gerenciados permitem a você dar suporte a determinadas políticas do Azure, fornecendo aos clientes maior confiança e conforto ao usar seus aplicativos. Além disso, você deve comprar e aplicar licenças da Microsoft, sua organização ou organizações que instalam seus aplicativos, para permitir que o aplicativo acesse os dados através do Data Connect.

## <a name="policies"></a>Políticas

As seguintes políticas do Azure são compatíveis com um desenvolvedor de aplicativo gerenciando do Azure usando dados do Office 365:

- [Política de Criptografia Necessária do ADLS Gen1](https://docs.microsoft.com/pt-BR/azure/azure-policy/scripts/enforce-datalakestore-encryption)

Ao selecionar qualquer uma das políticas durante a publicação do Azure Marketplace, o status de conformidade da política será marcado e aplicado a todas as instalações do seu aplicativo. Todas as políticas selecionadas compatíveis serão exibidas para os aprovadores de dados como parte da solicitação de dados. Qualquer violação de conformidade da política causaria falha no pipeline e interrupção da extração de dados.

Se deseja solicitar suporte para outras políticas, informe em [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581).

## <a name="licensing"></a>Licenças

Acesso ao conjunto de ferramentas do Microsoft Graph Data Connect disponível por meio do Workplace Analytics, que é licenciado por cada usuário, mensalmente.  Organizações com o Workplace Analytics podem estender suas informações de dados do Office 365 ao conceder e controlar o acesso aos seus dados em escala para aplicativos desenvolvidos internamente ou por fornecedores independentes de software (ISVs). Para saber mais, inclusive sobre como comprar, visite a [página de produto do Workplace Analytics](https://products.office.com/pt-BR/business/workplace-analytics).

Se você for um ISV, também fornecemos uma opção para desenvolver aplicativos para os clientes que não compraram o Workplace Analytics. Para fazer isso, você deve comprar licenças suficientes para associá-las com todos os usuários que o aplicativo acessará por meio do Microsoft Graph Data Connect, para cada cliente que compra o aplicativo. Você pode usar essa opção com licenças do Workplace Analytics. Você precisará executar etapas para associar as instâncias da licença do Microsoft Graph Data Connect com cada uma de suas instalações do cliente.

### <a name="isvs-using-the-microsoft-graph-data-connect-license"></a>ISVs usando licença do Microsoft Graph Data Connect
Se você for um ISV usando licença do Data Connect, você deve usar [Azure Key Vault](https://azure.microsoft.com/pt-BR/services/key-vault/) para armazenar e processar a atribuição de licença. Será preciso [criar um Key Vault](https://docs.microsoft.com/pt-BR/azure/key-vault/quick-create-portal). Durante a criação, anote o valor URI do Key Vault. Ele será usado na definição de aplicativo para fazer referência ao Key Vault. Após criar o Key Vault, certifique-se de que o SPN usado no Serviço Vinculado à Fonte do modelo ARM do aplicativo tenha acesso a ele. Para fazer isso, acesse o painel **políticas de acesso** da instância do Key Vault, crie uma política de acesso para o aplicativo referenciada pelo SPN, e atribua permissões ao aplicativo em **Obter** e **Lista**. 

![Criar política de acesso ao Key Vault](images/data-connect-keyvault-access.png)

A atribuição das licenças do Microsoft Graph Data Connect para as organizações é fornecido como um segredo no Key Vault. Para fazer isso:
1. No Key Vault, clique em **Gerar/Importar**, e crie um segredo manual. O nome do segredo deve ser **MGdcSKUMapping** e o valor do segredo deve conter a ID de locatário e o número de licenças alocado para esse locatário, no formato a seguir.

`{"tenantId1" : 20, "tenantId2" : 35, "tenantId3" : 12}`

2. Após configurar o valor, verifique se está habilitado e selecione **Criar** para iniciar a implantação. 

![Criar o segredo no Key Vault](images/data-connect-keyvault-create.png)

3. Você também precisa atualizar o modelo ARM do aplicativo para fazer referência ao Key Vault que você criou. Para fazer isso, preencha as propriedades do **LicenseKeyVaultUri**, que devem ser preenchidas com o valor **KeyVaultUri** que você anotou durante a criação. Essa propriedade é fornecida no Serviço Vinculado à Fonte do modelo ARM do aplicativo, conforme mostrado. 

```
"properties": {
        "type": "Office365",
            "description": "Source O365 linked service",
            "typeProperties": {
                   "office365tenantId": "[subscription().tenantId]",
        "PrivacyPolicyUri": "http://www.wkw.com/privacy",
        "TermsOfUseUri": "http://www.wkw.com/tos",
        "servicePrincipalId": "[variables('sourceLinkedServicePrincipalId')]",
        "servicePrincipalKey": {
                           "type": "SecureString",
                "value": "[variables('sourceLinkedServicePrincipalKey')]"
        },
        "servicePrincipalTenantId": "[variables('sourceLinkedServicePrincipalTenantId')]",
        "LicenseKeyVaultUri": "<KeyVaultUri>",
            }
    }
```

Data Connect fará referência ao segredo do Key Vault antes de executar cada pipeline. O pipeline irá falhar se não houver licenças suficientes atribuídas à organização para fornecer dados para cada usuário ou se o Key Vault estiver inacessível. 

## <a name="next-steps"></a>Próximos passos
Se deseja solicitar suporte para outras políticas, informe em [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581). Para saber mais sobre Workplace Analytics, inclusive sobre como comprar, visite a [página de produto do Workplace Analytics](https://products.office.com/pt-BR/business/workplace-analytics).
