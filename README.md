unsolved tasks

index.tsx

type UserWalletType = {
title: string
amount: number
}
type UserWalletPropsType = {
wallet: UserWalletType
}

export const UserWallet: React.FC<UserWalletPropsType> = (props) => {
return <div>title: {props.wallet.title}, amount: {props.wallet.amount}</div>
}

export const UserMoney = (props: UserWalletPropsType) => {
const wallets = [
{title: 'bitcoin', amount: 1},
{title: '$', amount: 100}
]

    return <div>
        <UserWallet wallet={} />
        <UserWallet wallet={} />
    </div>
}